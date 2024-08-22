```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Git as Git
    Dev->>Git: git checkout <target-branch>
    Dev->>Git: git cherry-pick <commit-hash>
    Git->>Dev: Commit applied
    Dev->>Git: Resolve conflicts if any
    Dev->>Git: git commit
    Dev->>Git: git push
