```mermaid
graph TD
    A[git submodule add &lt repository-url &gt] --> B[git submodule update --init --recursive]
    B --> C[git commit -m 'Added submodule']
