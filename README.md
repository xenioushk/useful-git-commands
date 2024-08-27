# Useful & Frequently Userd git Commands

This documentation provides a quick setup process of Git and a few useful commands.

## Git Setup

- Download git application from https://git-scm.com
- install it on your computer.
- Open the terminal(Mac) or Poweshell (Windows).
- Once done, run the following command to check the git version.

```bash
git --version
```

## Last 3 Git Logs

```bash
git log -3
```

## Git Logs in Graphical Mode

```bash
git log --graph
```

## Setup Git User Name and Email

```bash
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```

### Validate user information

```bash
git config --global user.name
git config --global user.email
```

<h3>Git Push & Pull Commands</h3>

```bash
git init

git status

git add -A

git commit -m "your_custom_commit_message_in_here"

git commit -am "your custom_commit_message_in_here"

git remote add origin "git_remote_repository_url"

//set upstream. (rename the remote from origin to upstream)

git remote rename origin upstream

// Using -u, you can set the upstream branch for the current branch. e.g main
git push -u origin main

// Pull any changes from remote main branch
git pull origin main

git clone "git_remote_repository_url"

git reset "index.html"

// Check current origin
git remote -v

//Set a new origin.
git remote set-url origin "git_remote_repository_url"
```

## Git Branch Commands

```bash

// List of all branches.
git branch -a

// Create a new branch and switch to that branch
git checkout -b "new_branch_name"

//Rename current branch.
git branch -m "new_renamed_branch_name"

// delete a branch.
git branch -d "deleted_branch_name"

//switch to a branch.
git checkout "branch_name"

// merge a branch.
git merge "branch_name"

// Check branch logs
git log --oneline
```

## Fix fatal: refusing to merge unrelated histories issue

- Run the following command. (Check origin name, for mine it's the main)

  ```bash
  git pull origin main --allow-unrelated-histories
  ```

- After running this code a popup window will appear. Press 'wq' from keyboard.
- It's done. Now you can push your code to the remote repository.

<h3>Bonus Commands For Mac </h3>

1. Create a new directory

```bash
mkdir YOUR_DIR_NAME
```

2. Create an empty file.

```bash
touch YOUR_FILE_NAME
```

3. Read A File.

```bash
cat YOUR_FILE_NAME
```

## Bonus Commands For Windows

1. Create a directory

```bash
mkdir YOUR_DIR_NAME
```

2. List of folder and files in a directory.

```bash
ls YOUR_DIR_NAME
```

3. Create an empty file.

```bash
echo YOUR_FILE_NAME
```
