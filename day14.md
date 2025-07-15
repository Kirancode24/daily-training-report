## Traninig Day :- 14

### Branching, Remote Operations & GitHub/GitLab Basics

---

####  Branching and Merging in Git

#####  What is Branching?
Branching means creating a **separate line of development**. It helps developers to work on features or fixes independently, without affecting the main code.

#### Features of Branching
- Isolates development work (feature, bug fix, etc.)
- Allows multiple people to work simultaneously
- Helps avoid conflicts
- Can be merged into the main branch
- Lightweight and fast

####  Simple Analogy

> Think of Git as a tree:
> - The `main` branch is the **trunk**.
> - New branches are **limbs** growing off the trunk.
> - Work is done on the limb, then **merged back** into the trunk.

---

#### Steps to Perform Branching in Git

> Example Folder: `Practice`

##### 1. Create a New Branch
```bash
git branch my-feature
````

##### 2. Switch to the New Branch (Checkout)

```bash
git checkout my-feature
```

 Or create and switch in one step:

```bash
git checkout -b my-feature
```

##### 3. Do Work → Add Changes → Commit

```bash
git add .
git commit -m "Added feature X"
```

##### 4. Switch Back to Main Branch

```bash
git checkout main
```

##### 5. Merge Feature Branch into Main

```bash
git merge my-feature
```

 Now your feature is merged into the main project.

---

####  Merging in Git

* Combines changes from one branch into another.
* May result in **merge conflicts**, which must be resolved manually.
* Helps integrate completed features into the main project.

##### Merge command :

 git checkout main
 git merge feature-branch
 
---

#### Remote Operations in Git

#####  `git push`

Sends your local commits to the remote repository.

```bash
git push origin main
```

#####  `git pull`

Fetches changes from the remote and merges into your local branch.

```bash
git pull origin main
```




#####  `git remote`

Manages remote repository connections.

```bash
git remote -v
```



---

#### GitHub / GitLab Basics

#####  What are GitHub and GitLab?

* Online platforms that **host Git repositories**.
* Provide features like:

  * Pull/Merge Requests
  * Issue Tracking
  * Collaboration Tools
  * CI/CD Integration

#####  Common Uses

* Store and manage code online
* Collaborate on open-source and private projects
* Review code via Pull Requests (PRs)

---

#### Summary Commands

| Purpose          | Command Example               |
| ---------------- | ----------------------------- |
| Create branch    | `git branch new-feature`      |
| Switch branch    | `git checkout new-feature`    |
| Create & switch  | `git checkout -b new-feature` |
| Add changes      | `git add .`                   |
| Commit changes   | `git commit -m "Message"`     |
| Merge branches   | `git merge new-feature`       |
| Push to remote   | `git push origin branch-name` |
| Pull from remote | `git pull origin branch-name` |

---

 **Tip:** Always pull latest changes before starting new work:

```bash
git pull origin main
```

---
