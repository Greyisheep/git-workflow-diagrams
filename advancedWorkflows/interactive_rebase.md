```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Git as Git
    Dev->>Git: git rebase -i <commit-hash>
    Dev->>Git: Reorder/Edit/Squash commits
    Dev->>Git: git rebase --continue
