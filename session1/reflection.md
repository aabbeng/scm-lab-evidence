# Session 1 Reflection

## Q1. Why is commit history useful when maintaining software?

A commit history gives maintainers a dated sequence of small, named changes instead of one unexplained final folder. If a defect appeared after the `Add teammate file` change, I could compare that commit with `Add Session 1 notes` to see exactly what changed and decide whether to fix or revert it. The messages in this repository also make it easy to identify when the README, ignore rules, notes, and teammate file were introduced.

## Q2. What is the difference between Git and GitHub?

Git is the version-control program that recorded commits and branches in my local `scm-lab-evidence` folder. GitHub is the online service that hosts the remote copies of both `scm-lab-evidence` and `skills-introduction-to-github`. I could use Git locally without a network connection, while GitHub provided sharing, Actions checks, issues, and the pull request used by the exercise.

## Q3. Why use a branch and pull request instead of changing main directly?

Working on `my-first-branch` kept the new `PROFILE.md` change separate from the stable `main` branch. The pull request showed the exact proposed change and gave GitHub Actions a place to check it before it was merged. This reduces the risk of incomplete or incorrect work reaching the main line without review.

## Q4. Which commands changed only the computer, and which changed GitHub?

Commands such as `git init`, `git status`, `git add`, `git commit`, `git diff`, `git log`, `git switch`, `git merge`, `git branch -d`, and `git restore` changed or inspected only my local folders and repositories. `git remote add origin` only stored the GitHub address locally, while `git clone`, `git fetch`, and `git pull` downloaded information from GitHub to the computer. `git push` was the command that uploaded local commits or branch changes and therefore changed the GitHub repository.

## Concept table

| Term | Definition |
| --- | --- |
| Repository | A project folder together with the complete Git history used to track it. |
| Working tree | The checked-out files and folders that I can currently see and edit. |
| Staging area | The list of changes selected by `git add` for inclusion in the next commit. |
| Commit | A saved snapshot of staged changes with an author, date, and explanatory message. |
| Branch | A movable name pointing to a line of commits, allowing work to proceed separately. |
| Merge | The operation that combines changes from one branch into another branch. |
| Remote | A named reference to another copy of the repository, such as `origin` on GitHub. |
| Push | Upload local commits and branch updates to a remote repository. |
| Pull | Download remote commits and integrate them into the current local branch. |
| Clone | Create a new local copy of a remote repository, including its history. |

## Method

I used the Git command line in PowerShell for the local repository, branching, merging, pushing, cloning, and pulling steps.
