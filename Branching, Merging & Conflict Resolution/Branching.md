# Branching 101

Branches let you work on features, fixes, or experiments without affecting the main code. Here’s how to manage them.

---

## Core Branching Commands

- `git branch`  
  → Lists all local branches.  
  → Also creates a new branch if you add a name: `git branch <new-branch>`

- `git checkout -b <branch>`  
  → **Older syntax**: Creates a new branch *and* switches to it immediately.

- `git switch -c <branch>`  
  → **Modern syntax** (Git 2.23+): Creates a new branch and switches to it.  
  → Cleaner, more intuitive, and less error-prone.

- `git switch <branch>`  
  → Switches to an existing branch safely.  
  → Won’t let you switch if you have uncommitted changes that would be lost.

- `git branch -d <branch>`  
  → Deletes a branch.  
  → Only works if the branch is fully merged. Use `-D` to force-delete (e.g., `git branch -D <branch>`).

---

## Important Notes

> ⚠️ `git switch` is newer and more beginner-friendly.  
> It works only with Git versions 2.23 and later.

> ❗ `git branch` alone only *creates or lists* branches — it does **not** switch to them.

 



---

Tip: Always check which branch you’re on with `git branch` (look for the `*` next to the active branch).
