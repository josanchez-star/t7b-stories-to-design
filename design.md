```mermaid
Flowchart TD
A[Support Lead] --> B[Open Problems page]
B -->|Get /problems?status=open| C[API checks Request]
 C --> D[(Database: open problems)]
 D --> F[Sort by impact]
  F --> G[Ranked list shown to Support Lead]
  C -->|bad status| E[Error message]
  E --> A
  ```