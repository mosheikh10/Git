# Common Mistakes in the Real World

- Forgetting to `git pull` before pushing → can cause conflicts or overwrite others’ work.

- Force pushing (`git push --force`) to shared branches → dangerous! Only use if absolutely necessary and coordinated with the team.

- Committing secrets (API keys, passwords, tokens) → never commit sensitive data. Use environment variables or secret managers instead.

- Merging without review → bypasses quality control. Always get feedback via PRs before merging.

- Not using `.gitignore` properly → leads to committing unnecessary files (logs, build artifacts, IDE configs) or accidentally including secrets.

---

# Git at Scale

- **Monorepo strategies**  
  Manage multiple projects in one repo — simplifies dependencies and cross-project changes.

- **Sparse checkout**  
  Pull only specific directories/files from a large repo — saves time and disk space.

- **Large file support (Git LFS)**  
  Handle big files (images, videos, binaries) without bloating your repo.

- **Clean up legacy history**  
  Use `filter-branch` or `filter-repo` to rewrite or remove old/unused data from history.

- **Submodules vs subtrees in microservice repos**  
  Choose wisely: submodules link to other repos; subtrees embed them directly.

- **Selective CI builds** (e.g., Turborepo, Nx, Bazel)  
  Only run tests/builds for changed parts of the codebase — faster feedback.

- **Commit linting + bots to enforce rules**  
  Automate style, message format, or policy checks on every commit/PR.

- **GitOps-style deployments** (e.g., ArgoCD, Flux)  
  Treat infrastructure and app config as code — deploy by merging to main.

- **Server-side Git hooks** (e.g., `pre-commit.ci`, `Lefthook`)  
  Enforce quality, security, or formatting rules before commits are accepted.
