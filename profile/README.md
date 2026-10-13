# 🚀 Graduation Project – Practice & Sandbox Repository

Welcome to the official **Practice & Sandbox Repository** for our Graduation Project.

This repository is designed for **learning, experimentation, and team collaboration** before development begins in the production repository.

Its purpose is to allow every team member to become comfortable with Git, GitHub workflows, project structure, and our technology stack without risking production code.

> **Important**
>
> This is **NOT** the final project repository.
>
> Code in this repository may be rewritten, refactored, or discarded once development officially begins.

---

# 📌 Repository Goals

This repository is used to:

* Practice professional Git workflows
* Learn team collaboration using GitHub
* Test libraries, frameworks, and APIs
* Share research and documentation
* Experiment safely before production
* Learn how to create Pull Requests and resolve merge conflicts

---

# 🛠️ Technology Stack

Update this section once the final technologies are selected.

| Layer           | Technology                      |
| --------------- | ------------------------------- |
| AI Engine       | Python / PyTorch / TensorFlow   |
| Backend         | FastAPI / .NET / Spring Boot |
| Frontend        | React / Next.js / Vue           |
| Mobile          | Flutter / React Native          |
| Database        | PostgreSQL / MySQL / MongoDB    |
| Version Control | Git & GitHub                    |

---

# 🌿 Repository Branch Structure

The repository follows a department-based branching strategy.

```
main
│
├── dev/ai
├── dev/backend
├── dev/frontend
└── dev/mobile
```

## Branches

### `main`

* Stable production-ready practice code
* Protected branch
* No direct commits

---

### Department Branches

```
dev/ai
dev/backend
dev/frontend
dev/mobile
```

Each department works inside its own base branch.

Only reviewed Pull Requests are merged into these branches.

---

### dev Branches

Every contributor work on their own branch from the department branch.

* main
* dev/ai
* dev/backend
* dev/frontend
* dev/mobile

---

# 🚀 Development Workflow

## 1. Clone the Repository

```bash
git clone <repository-url>

cd Graduation-Project-Practice
```

---

## 2. Download Latest Branches

```bash
git fetch origin
```

---

## 3. Switch to Your Department Branch

Example for Backend developers:

```bash
git checkout dev/backend
git pull origin dev/backend
```

---

## 5. Develop Your dev

Write your code normally.

Check your work frequently:

```bash
git status
```

---

## 6. Stage Your Changes

```bash
git add .
```

or

```bash
git add filename
```

---

## 7. Commit

Use meaningful commit messages.

Good examples:

```text
feat: implement login endpoint

fix: resolve authentication bug

docs: update README

refactor: simplify tracker pipeline

test: add API unit tests

chore: update dependencies
```

---

## 8. Push Your Branch

```bash
git push origin dev/backend-ahmed-authentication
```

---

**Do NOT merge directly into `main`.**

---

# 🔄 Keeping Your Branch Updated

If your department branch changes while you're working:

```bash
git checkout dev/backend
git fetch origin

git merge origin/dev/backend
```

Resolve conflicts if necessary.

---

# 🛑 Resolving Merge Conflicts

If Git reports a conflict:

1. Open the conflicted file.
2. Decide which changes to keep.
3. Remove conflict markers.
4. Save the file.

Then run:

```bash
git add .

git commit -m "fix: resolve merge conflict"
```

---

# 🧹 Cleaning Up After Merge

After your Pull Request has been merged:

```bash
git checkout dev/backend

git pull origin dev/backend

git branch -d dev/backend-ahmed-authentication

git push origin --delete dev/backend-ahmed-authentication
```

---

# 📅 Daily Workflow

## 🌞 Start of the Day

```bash
git checkout dev/backend

git pull origin dev/backend

git checkout -b dev/backend-yourname-task
```

---

## 💻 During Development

```bash
git status

git add .

git commit -m "feat: implement dev"

git push origin dev/backend-yourname-task
```

Push regularly to avoid losing work.

---

## 🌙 Before Leaving

* Push all changes
* Update your Pull Request
* Ensure the project builds correctly
* Inform teammates if your work affects theirs

---

# 📖 Git Command Cheat Sheet

| Command                           | Purpose                 |
| --------------------------------- | ----------------------- |
| `git status`                      | Show current changes    |
| `git branch -a`                   | List all branches       |
| `git log --oneline --graph --all` | View commit history     |
| `git fetch origin`                | Download remote updates |
| `git pull origin <branch>`        | Pull latest changes     |
| `git checkout <branch>`           | Switch branches         |
| `git checkout -b <branch>`        | Create new branch       |
| `git add .`                       | Stage all changes       |
| `git commit -m "message"`         | Commit changes          |
| `git push origin <branch>`        | Push branch             |
| `git merge <branch>`              | Merge another branch    |
| `git branch -d <branch>`          | Delete local branch     |

---

# 💡 Best Practices

✅ Pull before starting work.
✅ Commit small logical changes.
✅ Push regularly.
✅ Keep commit messages meaningful.
✅ Review your code before opening a Pull Request.
✅ Test your code before pushing.
✅ Delete merged dev branches.

---

# 🚫 Things to Avoid

❌ Never commit directly to `main`.
❌ Never upload:
* `.env`
* `node_modules`
* Python virtual environments (`venv/`)
* compiled files
* temporary files
* IDE settings unless shared intentionally

---

# 📂 Recommended Repository Structure

```
Graduation-Project-Practice/

│── README.md
│── .gitignore
│
├── docs/
├── research/
├── ai/
├── backend/
├── frontend/
├── mobile/
├── datasets/
└── experiments/
```

---

# 🤝 Collaboration Rules

* Respect the branching strategy.
* Review teammates' Pull Requests carefully.
* Keep discussions constructive.
* Ask questions when unsure.
* Communicate before making major architectural changes.

---

# 🎯 Final Reminder

This repository exists to **learn**, **experiment**, and **collaborate**.

Mistakes are expected here—that is the purpose of this practice repository. Build good Git habits now so the transition to the production repository is smooth and efficient.
