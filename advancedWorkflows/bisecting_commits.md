```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Git as Git
    Dev->>Git: git bisect start
    Dev->>Git: git bisect bad
    Dev->>Git: git bisect good <commit>
    Dev->>Git: Run tests to find bad commit
    Dev->>Git: git bisect reset
