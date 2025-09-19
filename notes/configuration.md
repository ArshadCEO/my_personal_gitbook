[⬅️ Back to Index](../readme.md)

# ⚙️ Git Configuration  

After installing Git, the first step is to configure some essential settings. These configurations make sure your commits and workflow are set up properly.

The `--global` flag in Git simply means:

👉 **“Apply this setting to me, on this computer, for all my repositories.”**

So:

* If you use `--global`, the setting goes into your **global config file** (`~/.gitconfig`) and affects every repository you work on.
* If you don’t use `--global`, the setting applies **only to the current repository**.

## 1. Set User Information  

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```
👉 This information will appear as the author of your commits.

## 2. Set Default Branch Name

```bash
git config --global init.defaultBranch main
```

> In the past, **`master`** was used as the default branch name in Git.  
> Nowadays, you’ll more commonly see **`main`** as the default branch name.

---

➡️ Next: [Git Basic](./git_basic.md)
