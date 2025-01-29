# Version Control - Git & GitHub  

✨ **New to Git & GitHub?** No worries! This guide walks you through everything **step-by-step** from basic commands to working with repositories.  

---

## 📌 Index:  

### 🖥 Git (Local Version Control)  
1. **[Windows Command Prompt - Essential Commands 🔻](#-windows-command-prompt---essential-commands)**  
2. **[Git - Core Commands 🔻](#-git---core-commands)**  
3. **[Git - Working with Branches 🔻](#-git---working-with-branches)**  
4. **[Git - Deleting Branches 🔻](#-git---deleting-branches)**  

### 🌍 GitHub (Online Repository Management)  
5. **[GitHub - Adding Files 🔻](#-github---adding-files)**  
6. **[GitHub - Cloning a Repository 🔻](#-github---cloning-a-repository)**  
7. **[GitHub - Personal Access Tokens (PATs) 🔻](#-github---personal-access-tokens-pats)**  
8. **[GitHub - Collaborating on Projects 🔻](#-github---collaborating-on-projects)**  
9. **[GitHub - Forking and Pull Requests 🔻](#-github---forking-and-pull-requests)**  

---

## 🖥 Windows Command Prompt - Essential Commands  

### GUI vs CLI  
- **GUI (Graphical User Interface)** → Uses menus, buttons, and windows (e.g., File Explorer).  
- **CLI (Command Line Interface)** → Uses text-based commands (e.g., Command Prompt, Terminal).  

### 💡 Basic Command Line Navigation  

| **Command**               | **Action**                                   | **Example**                      |
|---------------------------|---------------------------------------------|----------------------------------|
| `dir`                     | List files and folders                      | `dir`                            |
| `cd folder-name`          | Move into a folder                          | `cd Projects`                    |
| `cd ..`                   | Move up one level                           | `cd ..`                          |
| `D:`                      | Switch to another drive                     | `D:`                             |
| `mkdir folder-name`       | Create a new folder                         | `mkdir new-folder`               |
| `echo "text" > file.txt`  | Create a file with text                     | `echo "Hello" > hello.txt`       |
| `type file.txt`           | Display file contents                       | `type hello.txt`                 |
| `del file.txt`            | Delete a file                               | `del hello.txt`                  |
| `rmdir /s folder-name`    | Delete a folder and all contents            | `rmdir /s old-project`           |

**[🔝 Back to Top](#version-control---git--github)**  

---

## 🔧 Git - Core Commands  

### 1️⃣ Checking & Setting Up Git  
✅ **Check Git installation:**  
```bash
git --version
```  
✅ **Initialize a Git repository:**  
```bash
git init
```  
✅ **Check repository status:**  
```bash
git status
```  
✅ **Set username & email (required for commits):**  
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```  

---

### 2️⃣ Tracking Changes  
✅ **Stage a file for commit (prepare it to be saved):**  
```bash
git add filename.txt
```  
✅ **Stage all changes:**  
```bash
git add .
```  
✅ **Commit changes (save them with a message):**  
```bash
git commit -m "Your commit message"
```  
✅ **View commit history:**  
```bash
git log
```
*(Press `q` to exit log view.)*  

**[⬆ Back to Top](#version-control---git--github)**  

---

## 🌱 Git - Working with Branches  

Branches let you work on different features **without affecting the main code**.  

✅ **Create a new branch:**  
```bash
git checkout -b feature-branch
```  
✅ **Switch branches:**  
```bash
git checkout main
```  
✅ **List all branches:**  
```bash
git branch -a
```  
✅ **Merge changes from a branch into `main`:**  
1. Switch to `main`:  
   ```bash
   git checkout main
   ```
2. Merge branch:  
   ```bash
   git merge feature-branch
   ```
⚠️ **Handling Merge Conflicts?**  
- If Git detects conflicts, open the affected file and manually resolve issues.  

**[🔝 Back to Top](#version-control---git--github)**  

---

## 🗑 Git - Deleting Branches  

✅ **Delete a branch locally:**  
```bash
git branch -D branch-name
```  
✅ **Undo last commit (restore a deleted file):**  
```bash
git reset --hard HEAD~1
```  

**[🔝 Back to Top](#version-control---git--github)**  

---

## 🚀 GitHub - Adding Files  

✅ **Link local repo to GitHub:**  
```bash
git remote add origin https://github.com/username/repository.git
```  
✅ **Push code to GitHub:**  
```bash
git push -u origin main
```  

**[🔝 Back to Top](#version-control---git--github)**  

---

## 📂 GitHub - Cloning a Repository  

✅ **Copy the repository URL from GitHub** and clone it to your local machine:  
```bash
git clone https://github.com/username/repository.git
```  

**[🔝 Back to Top](#version-control---git--github)**  

---

## 🔑 GitHub - Personal Access Tokens (PATs)  

GitHub now **requires a PAT** instead of a password for authentication.  

### 🛠 How to Generate a PAT:  
1. Go to **GitHub** → Click on your profile picture.  
2. Navigate to **Settings** → **Developer settings** → **Personal Access Tokens (Classic)**.  
3. Click **Generate new token (classic)**.  
4. Set an **expiration date** & select the `repo` scope.  
5. Click **Generate Token** and **copy it**! *(You won’t see it again!)*  

### 🔄 Use PAT Instead of Password:  
When Git asks for a password, **paste the PAT** instead.  
```bash
git push origin main
```

🚨 **Never share your PAT!** Store it securely (e.g., in a password manager).  

**[🔝 Back to Top](#version-control---git--github)**  

---

## 🤝 GitHub - Collaborating on Projects  

### Steps to Work as a Team:  
1. Accept the **GitHub invitation** to the repository.  
2. **Clone the repository**:  
   ```bash
   git clone https://github.com/project-owner/repository.git
   ```
3. **Create a new branch & make changes**:  
   ```bash
   git checkout -b feature-branch
   ```
4. **Push your changes**:  
   ```bash
   git add .
   git commit -m "Added feature"
   git push origin feature-branch
   ```
5. **Create a Pull Request (PR)** on GitHub to merge your changes.  

**[🔝 Back to Top](#version-control---git--github)**  

---

## 🍴 GitHub - Forking and Pull Requests  

✅ **Fork the repository** (if you don’t have direct access).  
✅ **Clone your fork**:  
```bash
git clone https://github.com/your-username/repository.git
```  
✅ **Sync with the original repository**:  
```bash
git remote add upstream https://github.com/original-owner/repository.git
```  
✅ **Make changes, push & submit a Pull Request**:  
```bash
git checkout -b fix-bug
git add .
git commit -m "Fix critical bug"
git push origin fix-bug
```  

🎉 **Done!** The original repository owner will review your PR.  

**[🔝 Back to Top](#version-control---git--github)**  
