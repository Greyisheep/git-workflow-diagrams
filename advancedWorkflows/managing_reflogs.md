```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Git as Git
    Dev->>Git: git reflog
    Git->>Dev: Shows commit history
    Dev->>Git: Identify the commit to reset
    Dev->>Git: git reset --hard <commit-hash>
