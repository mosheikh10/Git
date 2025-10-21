# Viewing Git History

Git gives you powerful tools to explore your project’s past. Here’s how to navigate and inspect your commit history.

---

## Core Commands

- `git log`  
  → Shows the full commit history: author, date, commit message, and hash.

- `git log --oneline --graph`  
  → Gives a compact, visual summary of commits and branches. Great for seeing branching/merging at a glance.

- `git show <commit>`  
  → Displays the full details of a specific commit (changes, author, message). Replace `<commit>` with the commit hash or reference (e.g., `HEAD~2`).

- `git diff`  
  → Compares **unstaged changes** (in Working Directory) vs the **last commit** (Repository). Shows what you’ve changed but not yet staged.

- `git diff --staged`  
  → Compares **staged changes** (in Staging Area) vs the **last commit**. Shows what you’re about to commit.

---

##  Bonus Commands

- `git blame <file>`  
  → Shows who last modified each line in a file, and when. Super useful for tracking down why a change was made.

- `git reflog`  
  → Shows your local **HEAD history**, including commits from deleted branches or lost work. Think of it as Git’s “undo history” — invaluable for recovery!


