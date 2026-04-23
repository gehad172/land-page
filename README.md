# 🌿 Git Workflow Guide

This guide explains how to create a new branch, push changes, and merge them into the `main` branch.

## 📌 Prerequisites

- Git installed on your machine
- Access to the repository
- Proper permissions to push and merge

---

## 🚀 Step 1: Clone the Repository (if not already)

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

---

## 🌱 Step 2: Create a New Branch

Create and switch to a new branch:

```bash
git checkout -b feature/your-branch-name
```

> 🔹 Use meaningful names like `feature/login-page` or `fix/navbar-bug`

---

## ✏️ Step 3: Make Your Changes

Edit your files, then stage and commit:

```bash
git add .
git commit -m "Add: meaningful description of your changes"
```

---

## 📤 Step 4: Push the Branch to Remote

```bash
git push origin feature/your-branch-name
```

---

## 🔀 Step 5: Merge into `main` Branch

### Option A: Using GitHub (Recommended)

1. Go to your repository on GitHub
2. Click **"Compare & pull request"**
3. Add description and submit PR
4. Review → Click **"Merge pull request"**

---

### Option B: Using Git CLI

Switch to main and pull latest changes:

```bash
git checkout main
git pull origin main
```

Merge your branch:

```bash
git merge feature/your-branch-name
```

Push updated main:

```bash
git push origin main
```

---

## 🧹 Step 6: Delete the Branch (Optional)

After merging:

```bash
git branch -d feature/your-branch-name
git push origin --delete feature/your-branch-name
```

---

## ✅ Best Practices

- Always pull latest `main` before creating a branch
- Keep branches small and focused
- Write clear commit messages
- Use Pull Requests for review
- Resolve conflicts carefully

---

## 📎 Example Workflow Summary

```bash
git checkout -b feature/new-feature
# make changes
git add .
git commit -m "Add new feature"
git push origin feature/new-feature
# open PR → merge
```

---
