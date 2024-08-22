```mermaid
graph TD
    A[git filter-branch --tree-filter 'command' HEAD] --> B[Review changes]
    B --> C[git push --force]
