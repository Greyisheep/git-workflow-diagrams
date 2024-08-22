```mermaid
graph TD
    A[git submodule add <repository-url>] --> B[git submodule update --init --recursive]
    B --> C[git commit -m "Added submodule"]
