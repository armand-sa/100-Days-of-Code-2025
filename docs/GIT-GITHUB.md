# Version Control - Git & GitHub

## Index:

## Git:

1. **[Windows Command Prompt - Commands🔻](#windows-command-prompt---commands)**
2. **[Git - Commands🔻](#git---commands)**

## GitHub:

1. **[GitHub - Anatomy of an HTML element🔻](#anatomy-of-an-html-element)**



<br />

---

## Windows Command Prompt - Commands

### GUI and CLI

- **GUI** - Graphical User Interface - top window
  - **File Explorer** - file manager
- **CLI** - Command Line Interface - bottom window
  - **Command Prompt** - command line interface

![GUI and CLI](../assets/gui-and-cli.webp)  

### 1. See what is inside a folder

```cmd
dir
```    

![dir](../assets/dir.webp) 

### 2. One folder up

```cmd
cd ..
```   

### 3. Move into another drive

```cmd
D:
```    

### 4. Go from `C:\Users>` go to arman

***Below is relative paths***

```cmd
cd arman
```  

**Go to desktop from `C:\Users\arman>`**

```cmd
cd OneDrive\Desktop
```  

***Below is absolute paths (What developers use)***

```cmd
cd C:\Users\arman\OneDrive\Desktop
```  

**To go to C:\Users**

```cmd
cd C:\Users\
```   

### 5. Go to root directory

```cmd
cd /
```  

### 6. Clear the screen

```cmd
cls
```  

### 7. Create a new folder

```cmd
mkdir new-folder
```  

### 8. Create a new file with content of "Hello, Armand"

```cmd
echo "Hello, Armand" > new-file.txt
```  

### 9. To read the file content

```cmd
type new-file.txt
``` 

### 10. Delete a file

```cmd
del new-file.txt
``` 

### 11. Delete a folder

```cmd
rmdir new-folder
``` 

### 12. Delete a folder and all files inside it

```cmd
rmdir /s new-folder
``` 


<br />

**[Return to Top 🔝](#version-control---git--github)**

---

## Git - Commands


### 1. See what git version is installed

```bash
git --version
```    

### 2. Initialize a git repository

- ***A brand new folder open in vs code, open terminal and run:***

```bash
git init
```    

- ***See if project is now being run by git:***

```bash
git status
```    

- ***Add a file that should be tracked by git:***

```bash
git add index.html
```    

**Credentials check / update (Optional)**

- ***Get/check the user name and email:***

```bash
git config --global user.name
git config --global user.email
``` 

- ***Update the user name and email:***

```bash
git config --global user.name "Armand"
git config --global user.email "armand@example.com"
``` 

- ***See what files need to be committed:***

```bash
git status
``` 

- ***Displays the commit history of a Git repository:***

```bash
git log
``` 

- ***Exit commit history:***

```bash
q
``` 




<br />

**[Return to Top 🔝](#version-control---git--github)**

---