# AI Engineering

Focus: **reliable** LLM systems — not demos.

## Core pipeline

```
User ? Backend ? Prompt Builder ? OpenAI ? JSON Parser ? Database
```

## Capabilities

| Area | Practice |
| --- | --- |
| Prompt engineering | Versioned prompts, eval-friendly templates |
| Structured outputs | JSON schemas, validation before persist |
| Function / tool calling | Explicit tool contracts, timeouts, retries |
| Agents | Bounded loops, MCP tools, human-in-the-loop when needed |
| RAG | Chunking, retrieval quality, grounded responses |
| Voice | Retell AI and similar for voice agents |
| Automation | Job queues wrapping LLM steps for durability |

## Production rules

1. Never trust model output — parse and validate  
2. Persist inputs/outputs for audit and debugging  
3. Prefer deterministic post-processing over clever prompts alone  
4. Isolate LLM latency behind queues when UX allows  

Diagram: [`../assets/architecture/ai-workflow.svg`](../assets/architecture/ai-workflow.svg)
