```mermaid
graph TD
    A[Fork the Repository] --> B[Clone the Forked Repository: <br>`git clone &lt forked-repo-url &gt`]
    B --> C[Set Up Upstream Repository: <br>`git remote add upstream &lt original-repo-url &gt`]
    C --> D[Create a New Branch: <br>`git checkout -b &lt feature-branch-name &gt`]
    D --> E[Make Changes Locally]
    E --> F[Add Changes: <br>`git add .`<br>Commit Changes: <br>`git commit -m &lt message &gt`]
    F --> G{Open an Issue?}
    G -->|Yes| H[Write an Issue]
    G -->|No| I[Skip Issue]
    H --> I[Skip Issue]
    I --> J[Sync with Upstream Repository: <br>`git fetch upstream`]
    J --> K[Merge Changes: <br>`git merge upstream/main`]
    K --> L[Push Changes to Fork: <br>`git push origin &lt feature-branch-name &gt`]
    L --> M[Create Pull Request on GitHub]
