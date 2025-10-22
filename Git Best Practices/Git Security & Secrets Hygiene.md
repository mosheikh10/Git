# Git Security & Secrets Hygiene

- Prevent secret leaks in commits — never commit API keys, passwords, tokens, or config files with sensitive data.

- Use tools like `git-secrets` or `trufflehog` to scan your code (and history) for accidental secrets before they go public.

- Clean secrets from history — if you accidentally committed a secret, use `git filter-repo` or `BFG Repo-Cleaner` to remove it permanently.

- Audit repo contributors and logs — review who has access and what changes were made, especially after security incidents.
