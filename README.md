# Useful & Frequently Userd git Commands

<h3>Git Setup</h3>

<p>Download git application from https://git-scm.com and install it on your computer. Run the following command in your computer command prompt application.</p>

<pre>
git --version
</pre>



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

git add remote origin "git_remote_repository_url"

git push origin main 

git pull origin main

git clone "git_remote_repository_url"

git reset "index.html"

git remote -v

git remote set-url origin "git_remote_repository_url"
</pre>



<h3>Git Branch Commands</h3>

<pre>
git branch

git branch -b "new_branch_name"

git branch -m "new_renamed_branch_name"

git branch -d "deleted_branch_name"

git checkout "branch_name"

git merge "branch_name"
</pre>
