# 🚀 Advanced Git Commands

Here are some powerful but lesser-known Git commands that can boost your workflow.

---

## 1. `git reflog`
Recover lost commits, branches, or rebases.

```bash
git reflog
git checkout HEAD@{3}
```

---

## 2. `git bisect`
Find which commit introduced a bug using binary search.

```bash
git bisect start
git bisect bad
git bisect good <commit-hash>
```

---

## 3. `git clean`
Remove untracked files and directories safely.

```bash
git clean -fdn   # dry run
git clean -fd    # delete
```

---

## 4. `git shortlog -sn`
Show contributors ranked by commits.

```bash
git shortlog -sn
```

---

## 5. `git stash push -m "message"`
Save work-in-progress with a message.

```bash
git stash push -m "fix login bug"
git stash list
git stash apply stash@{0}
```

---

## 6. `git blame -L`
See who modified specific lines.

```bash
git blame -L 25,50 app.js
```

---

## 7. `git log --oneline --graph --decorate --all`
Visualize your commit history in a compact form.

```bash
git log --oneline --graph --decorate --all
```

---

## 8. `git cherry-pick`
Apply a single commit from another branch.

```bash
git cherry-pick <commit-hash>
```

---

## 9. `git grep`
Search inside tracked files quickly.

```bash
git grep "useEffect"
```

---

## 10. `git worktree`
Work on multiple branches simultaneously in separate directories.

```bash
git worktree add ../feature-branch feature-branch
```

---

💡 **Pro Tip:**  
Combine these with Git aliases in your config file (`~/.gitconfig`) for even faster use!
