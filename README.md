# Version_Control

## Table of Contents

1. [What is Version Control?](#what-is-version-control)
2. [Git vs GitHub](#git-vs-github)
3. [3 GitHub Alternatives](#3-github-alternatives)
4. [Git Fetch vs Git Pull](#git-fetch-vs-git-pull)
5. [Git Rebase](#git-rebase)
6. [Git Cherry-pick](#git-cherry-pick)

---

## What is Version Control?

Version control is a system that tracks changes made to files over time. It lets you save different versions of your work so you can go back to an earlier version if something breaks, see exactly what changed and when, and collaborate with others without overwriting each other's work. It's like a detailed history of every change ever made to a codebase, with the ability to rewind to any point in that history.

---

## Git vs GitHub

Git is a version control tool that runs on your local machine. It is what you use to track changes, create branches, commit and manage your code history entirely offline. It does not need the internet to work.

GitHub is a cloud platform that hosts Git repositories online. It takes everything Git tracks locally and gives it a home on the internet where it can be shared, backed up and collaborated on with other developers.

The simplest way to put it: Git is the tool, GitHub is where you store and share what the tool produces. You can use Git without GitHub but GitHub is useless without Git.

---

## 3 GitHub Alternatives

**1. GitLab**
GitLab is a web-based platform similar to GitHub that hosts Git repositories. It is popular among teams who want more built-in tools for deployment and automation without needing third-party integrations.

**2. Bitbucket**
Bitbucket is a repository hosting service by Atlassian. It is widely used by teams that already work with other Atlassian products like Jira and Trello since they integrate seamlessly together.

**3. Azure DevOps**
Azure DevOps is Microsoft's platform for hosting repositories and managing software development pipelines. It is commonly used by enterprise teams working within the Microsoft ecosystem.

---

## Git Fetch vs Git Pull

`git fetch` downloads changes from the remote repository to your local machine but does not merge them into your current branch. It lets you see what has changed on the remote without affecting your local code. You are essentially saying "show me what is new but do not change anything yet."

`git pull` does two things at once. It fetches the changes from the remote repository and immediately merges them into your current branch. It is the faster option when you are confident you want the latest changes applied to your work straight away.

---

## Git Rebase

Git rebase is a way of moving or combining a sequence of commits to a new base commit. In simple terms it takes the changes you made on your branch and replays them on top of another branch as if you had started your work from that point. It keeps the commit history clean and linear instead of cluttered with merge commits.

**Command:**

```bash
git rebase <branch name>
```

**Example:**

```bash
git rebase main
```

---

## Git Cherry-pick

Git cherry-pick allows you to pick a specific commit from one branch and apply it to another branch without merging the entire branch. It is useful when you need one particular change from a branch but are not ready to merge everything else that branch contains.

**Command:**

```bash
git cherry-pick <commit hash>
```

**Example:**

```bash
git cherry-pick a1b2c3d
```

For example Where `a1b2c3d` is the unique ID of the specific commit you want to apply.
