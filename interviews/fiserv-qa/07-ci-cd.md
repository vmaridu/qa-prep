# 🦊 07 - CI/CD & Source Control

## 📌 Overview

- CI/CD helps teams automate build, test, and deployment workflows.
- Git is the foundation for version control and collaboration.

## 🌿 Git Basics

- `git clone`
- `git checkout -b feature-name`
- `git add .`
- `git commit -m "message"`
- `git push`
- `git pull`
- `git merge`

## 🔄 Pull Requests / Merge Requests

- Review code changes
- Run tests before merging
- Keep branches small and focused

## ⚙️ GitLab CI/CD Example

```yaml
stages:
  - test

test:
  script:
    - mvn test
```
