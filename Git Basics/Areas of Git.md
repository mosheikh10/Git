<img width="622" height="348" alt="image" src="https://github.com/user-attachments/assets/36ce85a9-34e7-45e7-9962-8f1be553d968" />


# The 3 Areas of Git

Git organizes your project changes into three distinct areas. Understanding these helps you manage your workflow effectively.

---

## 1. Working Directory
> 📄 *Files you’re editing*

- This is your local project folder — where you create, edit, and delete files.
- Changes here are **untracked** until you stage them.
- Think of it as your “active workspace.”

---

## 2. Staging Area (Index)
> ✏️ *Changes marked for commit*

- A temporary holding area where you prepare changes before committing.
- You use `git add <file>` to move changes from the Working Directory to the Staging Area.
- Lets you choose exactly which changes go into your next commit — even if you’ve edited multiple files.

---

## 3. Repository (local .git)
> 📸 *Commit snapshots*

- The actual Git database, stored in the hidden `.git` folder.
- Each `git commit` saves a snapshot of everything in the Staging Area.
- These commits form your project’s history — you can go back to any point later.

---

## 🔄 Workflow Flow
  - [Working Directory] → git add → [Staging Area] → git commit → [Repository]



### How It Works:
1. Edit files in your **Working Directory**.
2. Use `git add` to select which changes you want to include in your next commit → moves them to the **Staging Area**.
3. Run `git commit` to permanently save those staged changes as a snapshot in your **Repository**.

✅ This flow gives you precise control over what gets saved and when.
