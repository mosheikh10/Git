# Git Stash & Pop

- `git stash`  
  Temporarily saves uncommitted changes (files you’ve modified but not yet staged or committed).

- `git stash list`  
  Shows all saved stashes — useful if you’ve stashed multiple times.

- `git stash apply`  
  Reapplies the most recent stash to your working directory. The stash stays saved in the list.

- `git stash pop`  
  Reapplies the latest stash AND deletes it from the stash list — one-step “apply and clean up”.

---

Use when:  
Switching branches mid-task — you’re not ready to commit, but need to move on.

💡 Great for:  
“I’m not ready to commit, but I need to switch branches right now.”
