# How Git Branching Works (A Beginner's Guide)

Git branching lets you work on new features or fixes without breaking your main code. Think of it as making a safe copy of your project to experiment on.

## What is a branch?

A branch is a separate line of development. Your default branch is usually called `main`. When you create a new branch, Git starts it from your current work, and any changes you make stay on that branch until you decide to merge them.

## Why use branches?

- **Safety:** your `main` branch always stays working.
- **Organization:** one branch per feature or bug fix.
- **Collaboration:** teammates can work in parallel without overwriting each other.

## Basic commands

Create and switch to a new branch:

    git switch -c add-login-page

See all branches (the current one has a `*`):

    git branch

Switch back to main:

    git switch main

## A simple workflow

1. Create a branch: `git switch -c fix-typo`
2. Make your changes and save them:

        git add .
        git commit -m "Fix typo in README"

3. Push the branch to GitHub: `git push -u origin fix-typo`
4. Open a pull request so others can review it.
5. Merge the pull request into `main`.

## Tips

- Use short, descriptive branch names like `fix-login-bug`.
- Delete branches after merging to keep your repo clean.
- Pull the latest `main` before starting a new branch.

## Summary

Branches let you experiment safely, keep your work organized, and collaborate smoothly. Once you get used to the create, commit, push, merge cycle, you'll use it every day.
