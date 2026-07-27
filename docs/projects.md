# Featured Projects

Polished placeholders — replace with verified metrics, links, and screenshots.

## Everest Railcar

**Domain:** Industrial / railcar operations  
**Role:** Full Stack / Backend architecture  

### Business problem

Fragmented railcar workflows made status tracking, ownership, and audits slow and error-prone.

### Solution

A role-based operations platform with APIs for status updates, audit trails, and real-time visibility for ops teams.

### Architecture highlights

- NestJS modular API with auth/RBAC  
- React client for operators and admins  
- PostgreSQL as system of record  
- Queue-backed jobs for heavy / async work  

### Stack

NestJS · React · PostgreSQL · Redis · AWS · Docker  

### Engineering challenges

- Access control across roles without blocking ops speed  
- Reliable status transitions and auditability  
- Background processing without blocking API latency  

### Impact

Faster operational cycles and clearer accountability in production workflows.

---

## ShackWise

**Domain:** Multi-site operations SaaS  
**Role:** Full Stack Architect  

### Business problem

Sites lacked a unified dashboard, reliable alerts, and consistent background processing.

### Solution

SaaS dashboards with async workers, caching, and notification pipelines.

### Architecture highlights

- Next.js for product UI  
- Node/Nest-style API layer  
- Redis for queues/cache  
- Dockerized deploy path  

### Stack

Next.js · Node.js · Redis · PostgreSQL · Docker · GitHub Actions  

### Impact

Centralized visibility and more reliable asynchronous workloads.

---

## Azara Healthcare

**Domain:** Healthcare workflows  
**Role:** Senior Software Engineer  

### Business problem

Sensitive care/ops workflows needed strict permissions, auditability, and secure cloud delivery.

### Solution

Secure application stack with RBAC, APIs, and AWS-aligned deployment.

### Architecture highlights

- React frontend  
- NestJS API  
- AWS (edge/API/storage patterns)  
- Durable relational storage  

### Stack

React · NestJS · PostgreSQL · AWS · Docker  

### Impact

Safer delivery of clinical/ops workflows with enforceable access boundaries.

---

## 5 Peaks Youth Solutions

**Domain:** Youth program management  
**Role:** Full Stack Engineer  

### Business problem

Program tracking, reporting, and staff coordination lived in disconnected tools.

### Solution

A central web platform for programs, reporting, and team coordination.

### Architecture highlights

- React SPA  
- Express API  
- MongoDB persistence  
- CI-friendly delivery  

### Stack

React · Express · MongoDB · CI/CD  

### Impact

Clearer reporting and operational coordination as program volume grows.
