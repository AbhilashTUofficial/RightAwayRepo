<details>
<summary>git version</summary>
<pre>
git --version
</pre>
</details>


<details>
<summary>Initialize git folder</summary>
<pre>
git init
</pre>
</details>


<details>
<summary>Add file to the track.</summary>
<pre>
git add readme.md
</pre>
</details>


<details>
<summary>Remove file from the track.</summary>
<pre>
git rm --cached readme.md
</pre>
</details>


<details>
<summary>Commit file to git</summary>
<pre>
git commit -m "message"
</pre>
</details>


<details>
<summary>Display all the stage and unstage files</summary>
<pre>
git status
</pre>
</details>


<details>
<summary>Discard all changes and restore the previous file.</summary>
<pre>
git restore readme.md
</pre>
</details>


<details>
<summary>See the diff</summary>
<pre>
git diff fileName
</pre>
</details>


<details>
<summary>Create a new branch and get to that branch</summary>
<pre>
git checkout -b newBranch
</pre>
</details>


<details>
<summary>checkout from the current branch and get to the master branch</summary>
<pre>
git checkout master
</pre>
</details>


<details>
<summary>merge changes from master to the current branch</summary>
<pre>
git merge master
</pre>
</details>

<details>
<summary>Clone from specific branch.</summary>
<pre>
git clone -b branchName url/ssh
</pre>
</details>

<details>
<summary>Initialize the username.</summary>
<pre>
git config --global user.name "username"
</pre>
</details>


<details>
<summary>initialize the email id.</summary>
<pre>
git config --global user.email email@gmail.com
</pre>
</details>

<details>
<summary>list the users</summary>
<pre>
git config --list --show-origin
</pre>
</details>

<details>
<summary>Get the log about the commit, including username, email, date, and time.</summary>
<pre>
git log
</pre>
</details>


