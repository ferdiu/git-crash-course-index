# Git crash course

### **1. What is Git? (Fast)**
- **Definition:** A distributed version control system.
- **Why use it?** Tracks changes, enables collaboration, and prevents data loss.
- **How it differs from other VCS?** (e.g., SVN, Mercurial)
- **Git vs. GitHub:** Briefly clarify the difference.

---

### **2. Git Features**
#### **Basic Features:**
- Repositories (`git init`, `git clone`)
- Commits (`git add`, `git commit`, `git log`)
- Branching (`git branch`, `git checkout`, `git switch`, `git merge`)
  - [Merge strategies](https://git-scm.com/docs/merge-strategies) (a brief introduction)
- Remote Repos (`git push`, `git pull`, `git fetch`)

#### **Some Advanced Features:**
- Interactive rebase (`git rebase -i`) for clean commit history
- Cherry-picking (`git cherry-pick`) for selective commits
- Stashing (`git stash`, `git stash pop`) for temporary changes
- Bisect (`git bisect`) to find bugs
- Hooks (`pre-commit`, `post-merge`)
- **Git Submodules** (`git submodule add`, `git submodule update`) for managing dependencies in large projects.

---

### **3. Best Practices for Working with Git**
#### **3a. Open Source Projects**
- Forking and cloning projects
- Pull requests (PRs) and code reviews
- Keeping your fork updated (`git rebase`, `git merge`)
- Contribution guidelines (commit messages, issue tracking)

#### **3b. Private/Team Projects**
- Branching strategy (Git Flow, GitHub Flow, Trunk-based)
- Feature branches and pull request workflow
- Code review policies
- Handling merge conflicts effectively

---

### **4. GitHub**
- Repositories, issues, and pull requests
- Actions and automation
- GitHub Pages for hosting
- Security features (Dependabot, code scanning)
- Projects

---

### **5. Introduction to CI/CD & Its Importance**
- **What is CI/CD?** Continuous Integration & Continuous Deployment
- **Why is it important?** Automates testing, deployment, and ensures reliability
- **How Git integrates with CI/CD?** GitHub Actions, GitLab CI/CD, Jenkins
- **Basic example of a GitHub Action workflow**

---

### **6. Bonus: Git Under the Hood (Exploring `.git/`)**
A quick look into how Git actually stores information:

- **Objects (`.git/objects/`)** – Where commits, trees, and blobs are stored
- **References (`.git/refs/`)** – Stores branches and tags
- **HEAD (`.git/HEAD`)** – Points to the current branch
- **Index (`.git/index`)** – The staging area
- **Config (`.git/config`)** – Repo-specific settings
- **Logs (`.git/logs/`)** – History of branch movements and HEAD changes

---

## Appendix

#### Main differences between VCSes

| **Feature**       | **Git** (Distributed) | **Mercurial** (Distributed) | **SVN** (Centralized) |
|--------------|----------------------|-------------------------|---------------------|
| **Repository Model** | Distributed (local copies) | Distributed (local copies) | Centralized (server-based) |
| **Branching**   | Lightweight, fast | Permanent, uses bookmarks | Heavy, slow |
| **Speed**       | Very fast | Fast but slower than Git | Slower |
| **History Model** | Snapshot-based | Snapshot-based | Changeset-based |
| **History Rewriting** | Allowed (`rebase`, `amend`) | Discouraged | Not possible |
| **Popularity**  | Very high | Declining | Low (but still in use) |
