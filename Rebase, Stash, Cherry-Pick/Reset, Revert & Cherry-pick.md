# Git Revert, Reset & Cherry-Pick

## 🟦 git revert
- Creates a *new* commit that undoes the changes of a previous commit.
- Safe for shared history (like production or team branches) — doesn’t rewrite history.
- Use when you need to undo something without breaking others’ work.

## 🟧 git reset
- Moves your branch pointer backward to an earlier commit.
  - `--soft`: keeps changes staged (ready to re-commit).
  - `--mixed` (default): unstages changes but keeps them in your working directory.
  - `--hard`: deletes all changes — use with caution!
- Rewrites history — best for local, unshared branches.

## 🟦 git cherry-pick
- Applies a *single* commit from one branch onto your current branch.
- Great for pulling specific fixes (like hotfixes) into another branch without merging everything.
- Useful for targeted changes — not whole branches.

  ---
  ## Explanation

git revert

Before:
A → B → C (bad commit)

Command:
git revert C

After:
A → B → C → C'

C' is a new commit that undoes C.
Safe for shared branches (doesn’t rewrite history).

---

git reset

Before:
A → B → C → D (current HEAD)

Command:
git reset --hard B

After:
A → B

Commits C and D are removed from history.
Rewrites history — only safe for local branches.

---

git cherry-pick

Before:
main: A → B
feature-login: A → B → C → D

Command (on main):
git cherry-pick D

After:
main: A → B → D'
feature-login: A → B → C → D

D' is a copy of D applied onto main.
Only that one commit is brought over — history stays clean.
