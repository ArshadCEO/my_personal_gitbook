# What is Git?

**Git** is a tool used by developers to **track versions of code and files**.  

Think of it like working on a document:  
- Every time you make changes, you save a new version (`file_v1`, `file_v2`, `final_file`, etc.).  
- This quickly becomes messy.  

Git solves this problem by:  
- ✅ Automatically saving each change as a **version**  
- ✅ Allowing you to **check old versions** anytime  
- ✅ Letting you **undo mistakes** easily  
- ✅ Helping multiple people work on the same project by **merging changes**  

👉 In short: **Git is like a time machine + teamwork tool for code and files.**

# How to Download and Install Git

Git can be installed on **Windows**, **macOS**, and **Linux** easily.  
Follow the steps below based on your operating system:

---

## 🖥️ Windows
1. Go to [Git for Windows](https://git-scm.com/download/win).  
2. Download the installer (`.exe` file).  
3. Run the installer and keep clicking **Next** (default options are fine).  
4. After installation, open **Command Prompt** or **Git Bash** and type:

   ```bash
   git --version
   ```

✅ If you see a version number, Git is installed successfully.

## 🍎 macOS
You can install Git in 3 ways:
1. Using Homebrew (recommended):

   ```bash
   brew install git
   ```
2. From the official website: [Git for mac](https://git-scm.com/download/mac).
3. Using Xcode Command Line Tools:
    ```bash
    xcode-select --install
    ```

## 🐧 Linux (Ubuntu/Debian)
1. Open Terminal and run:

    ```bash
    sudo apt update
    sudo apt install git
    ```
2. Verify installation:

   ```bash
   git --version
   ```

✅ Done!

Now Git is installed on your system and ready to use 🚀