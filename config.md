# Git Configuration Guide

## 1. User Information
Every Git commit stores your name and email.

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
````

## 2. Default Editor
Set the default editor for commit messages:

```bash
git config --global core.editor "code --wait"   # VS Code as default editor
```

## 3. Default Branch Name
Change the default branch from `master` to `main`:

```bash
git config --global init.defaultBranch main
```

## 4. Aliases (Shortcuts)
Create shortcuts for commonly used commands:

```bash
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.cm "commit -m"
```

## 5. Color Settings
Enable colored output for better readability:

```bash
git config --global color.ui auto
```

## 6. Merge Tool / Diff Tool
Use external merge or diff tools:

```bash
git config --global merge.tool vimdiff
git config --global diff.tool vimdiff
```

## 7. Credential Storage
Avoid typing username/password every time:

```bash
git config --global credential.helper cache
# or permanently store
git config --global credential.helper store
```

## 8. Check Configuration
List all your configurations:

```bash
git config --list
```

---

⚡ **Tips**

* `--global` → applies to your entire system (all repos)
* `--local` → applies only to the current repository
* `--system` → applies to all users on the system (admin level)
