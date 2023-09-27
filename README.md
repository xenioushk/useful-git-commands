# Useful & Frequently Userd git Commands

<h3>Git Setup</h3>

<p>Download git application from https://git-scm.com and install it on your computer. Run the following command in your computer command prompt application.</p>

<pre>
git --version
</pre>

<h3>Last 3 Git Logs</h3>

<pre>git log -3</pre>

<h3>Git Logs in Graphical Mode</h3>

<pre>git log --graph</pre>


<h3>Setup Git User Name and Email:</h3>

<pre>
git config --global user.name "Your Name"

git config --global user.email "Your Email"
</pre>

<p>Check the user information</p>

<pre>
git config --global user.name

git config --global user.email
</pre>



<h3>Git Push & Pull Commands</h3>

<pre>
git init

git status

git add -A

git commit -m "your_custom_commit_message_in_here"

git commit -am "your custom_commit_message_in_here"

git remote add origin "git_remote_repository_url"

git push origin main 

git pull origin main

git clone "git_remote_repository_url"

git reset "index.html"

//check current origin
git remote -v

//Set a new origin.
git remote set-url origin "git_remote_repository_url"
</pre>



<h3>Git Branch Commands</h3>

<pre>

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

// Check brach logs

git log --oneline
</pre>


<h3>Fix fatal: refusing to merge unrelated histories issue </h3>

1. Run the following command. (Check origin name, for mine it's the main)
2. <pre>git pull origin main --allow-unrelated-histories</pre>
3. After running this code a popup window will appear. Press 'wq' from keyboard.
4. It's done. Now you can push your code to the remote repository.

<h3>Bonus Commands For Mac </h3>

1. Create a directory.

<pre>echo YOUR_FILE_NAME</pre>

2. Create an empty file.

<pre>touch YOUR_FILE_NAME</pre>

3. Read A File.

<pre>cat YOUR_FILE_NAME</pre>

<h3>Bonus Commands For Windows </h3>

1. Create a directory

<pre>mkdir YOUR_DIR_NAME</pre>

2. List of folder and files in a directory.

<pre>ls YOUR_DIR_NAME</pre>

3. Create an empty file.

<pre>echo YOUR_FILE_NAME</pre>
