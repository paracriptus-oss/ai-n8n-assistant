# Диаграммы

```mermaid
flowchart LR
  A[Input] --> B[Preprocess]
  B --> C[LLM Request]
  C --> D[Postprocess]
  D --> E[Output]
