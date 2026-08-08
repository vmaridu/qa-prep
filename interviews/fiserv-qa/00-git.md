# 🌿 Git Tutorial for QA and Developers

## 📌 What is Git?

- Git is a distributed version control system.
- It helps teams track changes, collaborate, and manage code safely.
- It is used for source control in almost every modern software project.

---

## 🚀 1. Clone a Project

Clone means download a project from a remote repository.

```bash
git clone https://github.com/username/project.git
cd project
```

Example:

```bash
git clone https://github.com/example/qa-automation.git
cd qa-automation
```

---

## 🌿 2. Create a Branch

Branches let you work on features or fixes without affecting the main code.

```bash
git checkout -b feature/login-page
```

Or the newer syntax:

```bash
git switch -c feature/login-page
```

Example:

```bash
git switch -c bugfix/fix-login-test
```

---

## ✍️ 3. Make Changes and Commit

After editing files:

```bash
git status
git add .
git commit -m "Add login page test"
```

Real-world example:

```bash
git status
git add src/test/java/LoginTest.java
git commit -m "Add regression test for login flow"
```

---

## 🔄 4. Pull Changes

Before working, always check if others updated the branch.

```bash
git pull origin main
```

If you are on a feature branch:

```bash
git pull origin feature/login-page
```

If there are conflicts, resolve them carefully and commit again.

---

## ⬆️ 5. Push Changes

Send your branch to the remote repository.

```bash
git push origin feature/login-page
```

Example:

```bash
git push origin bugfix/fix-login-test
```

---

## 🔀 6. Pull Requests (PRs)

A pull request is a request to merge your branch into another branch, usually `main` or `develop`.

Typical workflow:

1. Create a branch
2. Make changes
3. Commit changes
4. Push branch
5. Open Pull Request
6. Team reviews the code
7. Merge after approval

Example:

```bash
git checkout -b feature/api-testing
# make changes
# commit
# push
```

Then open PR from `feature/api-testing` to `develop`.

---

## 🧭 7. Basic Branching Strategy

A common strategy is:

- `main` → production-ready code
- `develop` → integration branch for upcoming work
- `feature/*` → new features
- `bugfix/*` → fixes
- `hotfix/*` → urgent production fixes

### Example workflow

```bash
git switch develop
git pull origin develop
git switch -c feature/add-payment-test
# work and commit
# push branch
# create PR to develop
```

### Simple team branch model

```text
main
  └── develop
        ├── feature/login-flow
        ├── feature/api-tests
        └── bugfix/login-bug
```

---

## 🧑‍🤝‍🧑 8. How Teams Work with Git

Teams usually follow this flow:

1. Pull latest code from `develop` or `main`
2. Create a branch for the task
3. Make changes
4. Commit often with clear messages
5. Push the branch
6. Create a pull request
7. Review and approve
8. Merge into `develop` or `main`

### Example real-time project workflow

```bash
# 1. Start from latest develop

git switch develop
git pull origin develop

# 2. Create feature branch

git switch -c feature/add-api-automation

# 3. Work on files
# edit tests / code

# 4. Save changes

git status
git add .
git commit -m "Add API automation for user login"

# 5. Push feature branch

git push origin feature/add-api-automation

# 6. Open PR to develop
```

---

## 🛠️ 9. Useful Git Commands

```bash
git status

git log --oneline
git branch
git branch -a
git checkout <branch-name>
git switch <branch-name>
git merge <branch-name>
git stash
git stash pop
```

---

## ✅ 10. Best Practices

- Commit small, meaningful changes
- Use clear commit messages
- Pull before you push
- Keep branches short-lived
- Review code before merging
- Do not commit directly to `main` without review

---

## 🧠 Quick Summary

- Clone project → `git clone`
- Create branch → `git switch -c <branch>`
- Commit changes → `git add . && git commit -m "message"`
- Pull updates → `git pull`
- Push updates → `git push`
- Open PR → review and merge

---

## 📚 Example Team Flow

```text
Developer A:
- pulls latest develop
- creates feature branch
- writes tests
- pushes branch
- opens PR

Reviewer:
- checks code
- suggests changes
- approves PR

Team lead:
- merges PR into develop
- deploys after testing
```
