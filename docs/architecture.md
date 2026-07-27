# Architecture Notes

Systems I design repeatedly share the same production concerns: **boundaries**, **async work**, **data integrity**, and **operability**.

## Event-driven path

```
Client ? API ? BullMQ ? Redis ? Workers ? PostgreSQL
```

Use when:

- HTTP must stay fast while work is heavy or unreliable  
- Retries / backoff / concurrency limits matter  
- Multiple consumers need the same job stream  

## Cloud path

```
CloudFront ? Next.js ? NestJS ? Redis ? PostgreSQL ? AWS S3
```

Use when:

- Edge caching and static delivery improve UX  
- API and SPA need clear separation  
- Objects (uploads, exports) belong in S3, not the DB  

## Cross-cutting patterns

| Pattern | Intent |
| --- | --- |
| Auth + RBAC | Least privilege, auditable actions |
| Queues | Isolate failure, control throughput |
| Redis | Cache + broker for ephemeral state |
| Workers | Scale compute independently of API |
| Observability | Logs/metrics before outages escalate |

See diagrams in [`../assets/architecture/`](../assets/architecture/).
