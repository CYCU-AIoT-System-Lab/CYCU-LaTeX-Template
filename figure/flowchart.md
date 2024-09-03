```mermaid
flowchart LR

 a(Step A)
 b(Step B)
 c(Step C)
 d(Step D)
 e(Step E)

 subgraph Subprocess 1
 a-->b
 b-->c
 b-->d
 end
 
 subgraph Subprocess 2
 c-->e
 d-->e
 end
```
