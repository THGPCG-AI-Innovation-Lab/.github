# Contributing to GPCG Repositories

We appreciate your interest in contributing to one of our repositories. Please follow the steps below when contributing.

## Table of Contents

1. [Issue Tracking](#issue-tracking)
2. [Branching and Workflow](#branching-and-workflow)
3. [Code Reviews](#code-reviews)
4. [Atomic Commits](#atomic-commits)
5. [General Guidelines](#general-guidelines)

---

## Issue Tracking

1. Unless you are reporting a security vulnerability, **all** changes should start by **creating a GitHub Issue**:
   - Clearly describe the problem, enhancement, or suggestion.
   - Label the issue appropriately (e.g., "bug", "enhancement").
   - Assign the issue to yourself or the appropriate team member.
Always use a GitHub Issues Template if there is a suitable one available. Otherwise we do allow you to create a template free issue.
   
2. Once the issue is created, the associated branch should be named after the issue.

## Branching and Workflow

1. **Create a branch** named after the issue:
   ```bash
   git checkout -b issue-#issue_number-short-description
   ```
   For example, if the issue is #42 and it’s about improving documentation:
   ```bash
   git checkout -b issue-42-improve-docs
   ```
   You can do this directly from the GitHub Issue by clicking the _Create a branch from this issue_ link on the right hand side.
   
2. **Solve the issue on your branch**, ensuring the solution is isolated to the specific issue being addressed. Make sure you are working on the correct branch by checking out or changing the branch on GitHub (e.g. if you are working on the file using GitHub online)

3. **Push your branch** to the repository:
   
```bash
git push origin issue-#issue_number-short-description
```
4. Once the branch is ready, **submit a pull request**:

* Link the issue number in the pull request description.
* Ensure the pull request title is clear and descriptive.
* Assign reviewers if it’s a multi-developer project (see Code Reviews below).

## Code Reviews
For multi-developer projects, code reviews are required before merging any pull requests:

1. Assign at least one team member to review your pull request.

2. The reviewer will:
* Ensure the code solves the issue as described.
* Check for adherence to coding standards.
* Ensure that changes are atomic and not bundled with unrelated updates.

3. After the review, the reviewer may request changes or approve the pull request for merging.

## Atomic Commits
All contributions should be **atomic**:

* A commit should address only one issue or change. Avoid combining multiple unrelated changes into a single commit.
* Each commit should be small enough to describe a single change but large enough to solve the problem completely.

Example commit message:
```
fix: corrected typo in issue template
```
## General Guidelines

1. Adhere to the coding standards defined in the repository. Use meaningful commit messages and comments where necessary.
2. Test your changes to ensure they work as expected before submitting the pull request.
3. Follow the general workflow:
Log the issue → Create a branch → Solve the issue → Submit a pull request → Code review (if applicable) → Merge.
4. Maintain good documentation for any changes that affect workflows or processes within the repository.
5. Keep everything within scope: Ensure that your changes do not affect other unrelated files or processes.
---
Thank you for contributing! Your effort helps us maintain consistency and best practices across the organisation.
