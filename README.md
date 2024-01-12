# HTML FAQ Documentation

This repository contains HTML code for a Frequently Asked Questions (FAQ) page. The FAQ page is structured with questions and corresponding answers, providing information on version control, Git, GitHub, and related concepts.

## Version Control

A Version Control System (VCS) is a software tool that helps manage changes to source code over time. It allows multiple developers to work collaboratively on a project, tracking changes and coordinating updates to the codebase. The primary goals of a version control system include:

- **Tracking Changes:** VCS keeps a record of every change made to the source code, including details such as who made the change, when it was made, and a description of the change.

- **Collaboration:** Multiple developers can work on the same project simultaneously without interfering with each other's work. Changes made by one developer can be integrated with the work of others.

- **Branching and Merging:** VCS allows developers to create branches, which are separate lines of development. This is useful for working on new features or bug fixes without affecting the main codebase. Branches can later be merged back into the main branch.

- **Conflict Resolution:** When multiple developers make changes to the same part of the code simultaneously, conflicts may arise. VCS provides tools to resolve these conflicts and merge changes intelligently.

## Git vs GitHub

**Git:**
Git is a distributed version control system that is installed and runs locally on a developer's machine. Developers can create Git repositories on their local machines and work with version control without the need for an internet connection. It focuses on providing a command-line interface and a set of tools for managing repositories, branches, commits, and merges locally.

**GitHub:**
GitHub is a cloud-based platform that hosts Git repositories remotely on its servers. Developers can push their local Git repositories to GitHub, making them accessible to others. GitHub facilitates collaboration by providing a central platform for sharing and contributing to projects.

## GitHub Alternatives

1. **GitLab:**
   - Overview: GitLab is a web-based platform that provides Git repository management, continuous integration, and more. It offers both a cloud-based service (GitLab.com) and a self-hosted option (GitLab CE and GitLab EE) that can be installed on your own servers.

2. **Bitbucket:**
   - Overview: Bitbucket is a Git and Mercurial repository hosting service. It offers features like pull requests, code collaboration, and integration with other Atlassian products. Bitbucket is suitable for both small teams and large enterprises.

3. **SourceForge:**
   - Overview: SourceForge is an open-source platform that provides version control, bug tracking, collaboration tools, and more. It supports various version control systems, including Git, SVN, and Mercurial.

## Git Fetch vs Git Pull

- **git fetch:**
  Fetching is like asking Git to go to the remote repository and see if there are any changes. It retrieves the changes from the remote repository to your local repository but does not automatically merge these changes into your working directory.

- git pull:
  Pull is a combination of fetch and merge. It fetches changes from the remote repository and automatically merges them into your working directory. It brings the changes from the remote repository to your local repository and updates your working files to include those changes.

## Git Rebase

Imagine you have a feature branch where you've been working on some changes, and there have been new changes on the main branch (or another branch). Instead of merging those changes in (which creates additional merge commits), you can use git rebase to move your changes on top of the latest changes from the main branch. This makes the project history look more straightforward.

Basic command for git rebase:
```bash
git checkout your-feature-branch
git rebase target-branch
```

# Git Cherry-pickgit cherry-pick is used to apply a specific commit from one branch to another.
```bash
git cherry-pick <commit-hash>
