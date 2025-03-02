## Markdown
Markdown is a lightweight and easy-to-use syntax for styling your writing.

```
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

## GitHub Branches

### **1. What is a Branch?**  
- A **branch** is a parallel version of your code.  
- It allows multiple developers to work on different features without affecting the main codebase.  
- The default branch in most repositories is **main** or **master**.  
- Use branches to develop new features, fix bugs, or experiment safely.  

### **2. Creating a Branch**  
1. Open your GitHub repository.  
2. Click on the **branch dropdown** (next to the repository name).  
3. Type a new branch name and press **Enter**.  
4. Locally, create a branch using:  
   ```bash
   git checkout -b feature-branch
   ```  

## Pull Request

### **1. What is a Pull Request (PR)?**  
- A **Pull Request (PR)** is a request to merge changes from a branch into another (e.g., from `feature-branch` to `main`).  
- It allows for **code review**, discussions, and testing before merging.  

### **2. Creating a Pull Request**  
1. On GitHub, go to the repository → **Pull Requests** → **New Pull Request**.
2. Select the base branch (e.g., `main`) and compare it with your feature branch.  
3. Add a **title, description**, and mention reviewers.  
4. Click **Create Pull Request**.
5. Locally, push your branch to GitHub:  
   ```bash
   git push origin feature-branch
   ```  

### **3. Merging a Pull Request**  
- Once reviewed and approved:  
  - Click **Merge pull request** on GitHub.  
  - Locally, you can also merge using:  
    ```bash
    git checkout main
    git merge feature-branch
    ```  
- After merging, **delete the branch** to keep the repository clean:  
  ```bash
  git branch -d feature-branch
  git push origin --delete feature-branch
  ```
