- Combines changes from one branch into another.
- `git merge <branch>` → merges the specified branch into your current branch.
- Fast-forward vs recursive (true) merge — Git chooses automatically based on history.
- Creates a merge commit (unless it’s a fast-forward merge).
- May cause conflicts — requires manual resolution before completing the merge.


  <img width="430" height="172" alt="Screenshot 2025-10-21 at 01 47 02" src="https://github.com/user-attachments/assets/0af85b46-1a2e-4a5c-822a-c336d7b84050" />


  ---

  # Visualizing Branches & Logs

- `git log --oneline`  
  Shows each commit as a single line with its short hash and message — much easier to scan than the full log.

- `git log --graph`  
  Draws a simple ASCII graph (tree structure) showing how branches split and merge over time.

- `git log --oneline --graph --all`  
  The most useful combo: compact view + visual branching + includes **all** branches (not just the current one).

- These commands help you understand your repo’s structure, debug merge issues, and see where features or fixes came from.
