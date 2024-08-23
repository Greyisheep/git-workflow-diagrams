```mermaid
sequenceDiagram
    participant Dev as Developer
    participant Git as Git
    Dev->>Git: git stash
    Git->>Dev: Changes stashed
    Dev->>Git: git stash list
    Git->>Dev: Shows stashed changes
    Dev->>Git: git stash apply
    Git->>Dev: Applies stashed changes
    Dev->>Git: git stash drop
    Git->>Dev: Drops the stash
