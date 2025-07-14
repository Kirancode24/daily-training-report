## Training Day :- 13

### Introduction to Git and Version Control

---

## What is Git and Why Use Version Control?

###  What is Git?
**Git** is a **distributed version control system (VCS)** used to track changes in source code and collaborate on software projects. It helps developers work together efficiently, even on large and complex projects.

###  What is Version Control?
**Version control** is a system that records changes to a file or set of files over time, so you can recall specific versions later.

###  Benefits of Using Git & Version Control:
- Keep history of all changes.
- Collaborate with teams efficiently.
- Rollback to previous versions if something breaks.
- Work on multiple features simultaneously (branches).
- Avoid overwriting each other's work.

---
##  Why is Git Open Source?

Git is open-source because it is licensed under the **GNU General Public License (GPL)**. This allows anyone to **freely use, modify, and share** it. Being open-source encourages global collaboration, fast development, and secure improvements by the community.

---

##  Why Must Future Coders Learn Git?

Future coders must learn Git because it is a **crucial skill in software development**. It helps track code changes, supports **team collaboration**, ensures safe coding practices, and is widely used in the **tech industry**. Most coding jobs require Git knowledge.


## Git Architecture: Repository, Working Tree, Index

![alt text](gitarchi.jpg)

Git uses a **three-layer architecture**:

| Component              | Description |
|------------------------|-------------|
| **Repository (repo)**  | A `.git` directory that stores the entire history and configuration of the project. |
| **Working Tree**       | The current checked-out version of the project files (what you see and edit). |
| **Index (Staging Area)** | A space where changes are prepared before making a permanent commit. |

### Git Workflow Diagram:

Working Tree → Index (Staging Area) → Repository

---

###  Git with Command Line –


#### Step 1: Install Git

1. Go to the official Git website: [https://git-scm.com/](https://git-scm.com/)
2. Download Git based on your OS (Windows/Mac/Linux)
3. Install using the default options

 **Git download page or installation setup**

![alt text](git1.png)

![alt text](git2.png)

![alt text](git3.png)

![alt text](git4.png)

![alt text](git5.png)

#### Step 2: Create a GitHub Repository

1. Log in to [https://github.com](https://github.com)
2. Click on **New Repository**
3. Give your repo a name like `Practice`
4. Keep it **public**
5. Don't select **Initialize with README** if you are cloning from local
6. Click **Create repository**

 **Create repository page on GitHub**

![alt text](git6.png)

![alt text](git7.png)


####  Step 3: Clone Repository to Your System

Open **Git Bash** and use the command:

```bash
git clone https://github.com/kanikacoder13/Practice.git
```

##  Step 4: Go into the Project Folder

Use:

```bash
cd Practice
```

##  Step 5: Create a New File

Use this command:

```bash
touch index.html
```

![alt text](comm1.png)

![alt text](comm2.png)


##  Step 6: Edit the File

Edit using `nano` or VS Code or Notepad:

```bash
nano index.html
```

![alt text](comm3.png)


##  Step 7: Stage the File

Stage your file using:

```bash
git add index.html
```

##  Step 8: Commit Your Changes

Commit with a message:

```bash
git commit -m "Added index.html file"
```
![alt text](comm4.png)

##  Step 9: Push to GitHub

Now push to the GitHub repository:

```bash
git push origin main
```
![alt text](comm5.png)

![alt text](comm6.png)

![alt text](comm7.png)

![alt text](comm8.png)

![alt text](comm9.png)

-----

##  Core Git Operations (with Explanation)

### `git init`

* Initializes a new Git repository.
* Creates a `.git` folder to track the project.

```bash
git init
```

###  `git add`

* Adds files to the staging area (also called index).
* Prepares them to be committed.

```bash
git add filename      # Add a specific file
git add .             # Add all modified files
```

###  `git commit`

* Commits the staged changes to the Git repository.
* Every commit must have a message.

```bash
git commit -m "Your commit message"
```

###  `git status`

* Shows the status of files in the working directory and staging area.

```bash
git status
```

### `git log`

* Shows the commit history in reverse chronological order.

```bash
git log
```

![alt text](comm.png)

---

### GitHub Access & Personal Access Tokens

####  Why Use a Personal Access Token?

GitHub removed password authentication for Git. Use tokens for secure authentication instead.

####  How to Generate a Personal Access Token:

1. Go to **GitHub → Settings**
2. Open **Developer Settings**
3. Go to **Personal Access Tokens**
4. Click **Generate new token**
5. Set:

   * **Name of Token**
   * **Expiration Date**
   * **Permissions (Read/Write)**
6. Click **Generate**
7. **Copy the token** and keep it safe (you won’t see it again).

#### Never Share:

* API Keys
* Personal Tokens
* IP addresses
* Sensitive personal information

---

###  Do’s and Don’ts of GitHub

####  Do's

* Use `.gitignore` to skip unwanted files.
* Write clear, meaningful commit messages.
* Use branches to work on features separately.
* Push regularly to save progress online.

####  Don’ts

* Don’t share your **personal access tokens**.
* Don’t commit confidential data (API keys, passwords).
* Don’t edit code directly on the `main` branch without testing.

---

###  Summary of Git Commands

| Command                | Purpose                                  |
| ---------------------- | ---------------------------------------- |
| `git init`             | Create a new Git repository              |
| `git clone`            | Copy a remote repository to local system |
| `git add`              | Stage changes for commit                 |
| `git commit -m ""`     | Commit changes with a message            |
| `git status`           | View file status in working directory    |
| `git log`              | View commit history                      |
| `touch index.html`     | Create a new file                        |
| `nano index.html`      | Open and edit file in terminal           |
| `cd folder-name`       | Enter a folder                           |
| `ls`                   | List files in folder                     |
| `git push origin main` | Push commits to GitHub                   |

---
