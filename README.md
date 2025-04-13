# Useful & Frequently Used git Commands

This documentation provides a quick setup process of Git and a few useful commands.

## ✅ Git application setup

- Download git application from https://git-scm.com
- Install it on your computer.
- Open the terminal (Mac) or Poweshell (Windows).
- Once done, run the following command to check the git version.

```bash
git --version
```

or

```bash
git -v
```

**Output**

![git version check output](/previews/git_version_check_output.jpg)

## ✅ Setup git user name and email

```bash
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```

### Validate user information

```bash
git config --global user.name
git config --global user.email
```

### Initalize a git repository

```bash
git init
```

### Check git status

```bash
git status
```

### git push & pull commands

```bash

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

## ✅ Git branch commands

1. List of all branches.

```bash
git branch -a
```

2. Show current branch.

```bash
git branch --show-current
```

3. Create a new branch and switch to that branch

```bash
git checkout -b "new_branch_name"
```

4. Rename current branch.

```bash
git branch -m "new_renamed_branch_name"
```

5. Delete a branch. (locally)

```bash
git branch -d "deleted_branch_name"
```

6. Delete a branch. (remote)

```bash
git push origin -d "<BRANCH_NAME>"
```

7. Switch to a branch.

```bash
git checkout "branch_name"
```

8. Merge a branch.

```bash
git merge "branch_name"
```

## ✅ Git tag commands.

Using git tag commands you can easiliy mark stable version of a project. It creates an image of your git repository. To tag a branch, you need to checkout a stable branch. e.g `main`

```bash
git checkout branch "main"
git tag v1.0
```

### Add message to the tag

```bash
git tag -a v1.0 -m "this is a stable 1.0 version of my project"
```

### Show all the tags

```bash
git tag
```

### Push a tag

```bash
git push origin v1.0
```

### Push multiple tag

```bash
git push origin v1.0 v1.1
```

### Push all tags

```bash
git push --tags
```

### Delete a tag (local)

```bash
git tag -d v1.0
```

### Delete multiple tag (local)

```bash
git tag -d v1.0 v1.1
```

### Delete a tag (remote)

```bash
git push origin -d v1.0
```

## ✅ Git commit log

Using the following commands, you can check all previous commits hash, commits date, author.

### Check all logs

```bash
git log
```

### Last 3 git logs

```bash
git log -3
```

**Output**

![git version check output](/previews/git_last_3_logs.jpg)

## git logs in graphical mode

```bash
git log --graph
```

**Output**

![git version check output](/previews/git_log_graph_mode.jpg)

## git logs in oneline mode

```bash
git log --oneline
```

**Output**

![git version check output](/previews/git_log_oneline.jpg)

## Fix fatal: refusing to merge unrelated histories issue

- Run the following command. (Check origin name, for mine it's the main)

```bash
git pull origin main --allow-unrelated-histories
```

- After running this code a popup window will appear. Press 'wq' from keyboard.
- It's done. Now you can push your code to the remote repository.

## Remove a file/folder from git tracking

```bash
git rm -r --cached 'FOLDER_NAME'
```

## Update last git commit message.

If you accidentally added a Git commit message or would like to update the last Git commit message, then use the following command:

```bash
git commit --amend -m "Updated commit message"
```

### Bonus Commands For Mac

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

## Acknowledgement

- Md Mahbub Alam Khan

- [bluewindlab.net](https://bluewindlab.net)
