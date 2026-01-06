---
title: Intro to Git
---

## Intro

Git is the most popular version control system in the world. It allows you to track changes in your code, revert to previous versions, and collaborate with others.

## The Basic Workflow

The most common way to use Git involves three main stages: the **Working Directory**, the **Staging Area**, and the **Repository**.

### 1. Initialize a Repository

If you are starting a new project (not your blog, which is already a repo), you run:

```bash
git init
```

### 2. Check Status

Before you do anything, it's good to see what files have changed, you run:

```bash
git status
```

## The "Big Three" Commands

To save your work to internet (GitHub, GitLab, Bitbucket), you will almost always run these three commands in order.

### Step 1: Add (Stage)

Tell Git which files you want to save. To save everything, you run:

```bash
git add .
```

### Step 2: Commit (Save)

Take a "snapshot" of your project. Always include a clear message about what you changed, you run:

```bash
git commit -m "Add my new Git tutorial post"
```

### Step 3: Push (Upload)

Send your local saves to the internet (GitHub, GitLab, Bitbucket), you run:

```bash
git push origin main
```

## Helpful "Life Saver" Commands

| Command          | What it does                                                  |
| :--------------- | :------------------------------------------------------------ |
| `git clone`      | Downloading an existing project.                              |
| `git log`        | Shows your history of previous commits.                       |
| `git pull`       | Downloads the latest version from GitHub to your computer.    |
| `git checkout .` | **Be careful!** This undoes all changes since your last save. |

## Reference

- <https://git-scm.com/>
- <https://github.com/git-guides>
