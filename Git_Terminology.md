# Git Terminology and Commands

## Overview

Git is a version control system that allows you to track changes in your codebase, collaborate with others, and maintain a history of your project.

## CLI Commands

### Directory and File Management

- **Create a new directory:**

  ```bash
  mkdir <directory_name>
  ```

  > Creates a new directory in the current location.

- **Change the current directory:**

  ```bash
  cd <directory_name>
  ```

  > Moves into the specified directory.

- **Create a new file:**

  ```bash
  touch <file_name>.<extension>
  ```

  > Creates an empty file with the specified name and extension.

- **Remove a file:**

  ```bash
  rm <file_name>.<extension>
  ```

  > Deletes a file from the current directory.

- **Remove a directory and its contents:**

  ```bash
  rm -rf <directory_name>
  ```

  > Deletes a directory and all its contents.

- **List contents of a directory:**

  ```bash
  ls
  ```

  > Displays the files and folders in the current directory.

- **List all contents including hidden files:**

  ```bash
  ls -a
  ```

  > Shows all files, including hidden files starting with a dot (.).

- **Clear the terminal:**
  ```bash
  clear
  ```
  > Clears the terminal screen.

## Git Commands

### Initializing a Git Repository

- **Initialize a new Git repository:**
  ```bash
  git init
  ```
  > Sets up a new Git repository in the current directory.

### Checking Status

- **View repository status:**
  ```bash
  git status
  ```
  > Shows the state of the working directory and staging area, such as untracked files or changes ready to commit.

### Adding Files

- **Add a file to the staging area:**
  ```bash
  git add <file_name>.<extension>
  ```
  > Moves the specified file to the staging area in preparation for committing.

### Committing Changes

- **Commit staged changes:**
  ```bash
  git commit -m "Your commit message"
  ```
  > Records changes from the staging area to the repository with a descriptive message.

## Advanced Git Commands

### Stashing Changes

- **Save uncommitted changes for later:**

  ```bash
  git stash
  ```

  > Temporarily removes changes from the working directory, allowing you to work on other tasks.

- **View stashed changes:**
  ```bash
  git stash list
  ```
- **Apply stashed changes:**
  ```bash
  git stash apply
  ```

### Merging Branches

- **Merge a branch into the current branch:**
  ```bash
  git merge <branch_name>
  ```
  > Combines the specified branch into the current branch.

### Rebasing

- **Reapply commits on top of another base branch:**
  ```bash
  git rebase <branch_name>
  ```

### Resetting Changes

- **Undo changes in the working directory:**
  ```bash
  git reset <file_name>
  ```
  > Removes files from the staging area.
  - `--soft`: Keeps changes in the staging area.
  - `--mixed`: Removes changes from the staging area but keeps them in the working directory.
  - `--hard`: Discards all changes.

### Amending Commits

- **Edit the last commit message or add changes to it:**
  ```bash
  git commit --amend
  ```

### Pulling Changes

- **Download and merge changes from a remote repository:**
  ```bash
  git pull
  ```

### Tagging

- **Create a new tag:**
  ```bash
  git tag <tag_name>
  ```
- **Push a tag to a remote repository:**
  ```bash
  git push origin <tag_name>
  ```

### Undoing Changes

- **Revert a commit:**
  ```bash
  git revert <commit_hash>
  ```
- **Restore a file:**
  ```bash
  git restore <file_name>
  ```

## Git Configuration

- **Set global username:**
  ```bash
  git config --global user.name "Your Name"
  ```
- **Set global email:**
  ```bash
  git config --global user.email "your.email@example.com"
  ```

## Working with Remotes

- **Add a remote repository:**
  ```bash
  git remote add origin <repository_url>
  ```
- **Push changes to a remote repository:**
  ```bash
  git push origin <branch_name>
  ```

## Git Ignore File

- **Ignoring Files and Directories:**
  - Ignore a specific file:
    ```
    file.txt
    ```
  - Ignore all files with a specific extension:
    ```
    *.log
    ```
  - Ignore all files in a directory:
    ```
    /logs/*
    ```

## Forks and Pull Requests

- **Forking a Repository:** A copy of a repository on GitHub to your account for making changes without affecting the original repository.
- **Pull Requests:** A request to merge your changes into the original repository.

## Git Workflow
- **Workflow:**
  - Create a new branch for your feature or bug fix.
  - Make changes and commit them.
  - Push your branch to your forked repository.
  - Create a pull request to merge your changes into the original repository.
  - Review and discuss changes with others.
  - Merge the pull request once approved.
  - Update your local repository with the latest changes from the original repository.
  - Repeat the process for additional features or bug fixes.

  
