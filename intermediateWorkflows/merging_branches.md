```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Git as Git
    Dev->>Git: git checkout main
    Dev->>Git: git merge <branch-name>
    Dev->>Git: Resolve conflicts if any
    Dev->>Git: git commit
    Dev->>Git: git push
