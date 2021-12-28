Using Git & Github example

#### You have configured a git account with your local system. For the first-time Git configuration, you use the following commands:
<pre>
git config --global user.name <yourusername>  <i># Using this, you will enter your GitHub username</i>

git config --global user.email <youremail@example.com>  <i># Using this, you will enter your GitHub username</i>
</pre>

#### For configuration, you follow the following steps:
<pre>
echo "# fraud_detection" >> README.md <i>#This command create a readme file and adds # fraud detection as contents in the file.</i>
git init
git add README.md
git commit -m "first commit"
git branch
git remote add origin https://github.com/sajankedia/fraud_detection.git
git push -u origin master
</pre>

#### basic shell commands
<pre>
ls -  lists all the directories in the current directory. In windows, dir is used instead of ls

cat <filename> - displays the content in the file

cd <directory name> - to navigate to the directory

pwd - present working directory
</pre>

#### three main stages:

<pre>
Modified: When you change any code in the file.

Staged: When we add the file using ‘git add’, it goes into the staging area.

Committed: When you commit all the changes in the files that were in the staging area. 
</pre>

#### Commands used

<pre>
git add .
git status
git commit -m “message”
git push -u origin master
</pre>

[Basic Git commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)

#### Flow in Github

![Flow in Github](https://github.com/scpowar/Fraud-Detection/blob/master/flow_in_github.png?raw=true)

#### Git Log

<pre>
This command shows you the commit details. 
It lists out the commits made in the repository in reverse-chronological order, that is, the most recent commits show up first. 
It shows commits with the following details:
1. The commit ID or SHA
2. Author’s name (who made the commit)
3. Date and time

- For a shorter version of git log, you have git log --oneline
</pre>

#### Git Revert and Reset

<pre>
git revert HEAD   <i># → Reverts the project to the previously committed version </i>

git reset --hard #commit_ID  <i># → To go back to a commit that was 3-4 commits back</i>

‘git revert’ will create another commit that shows that you are reverting back to the previous commit. 
‘git reset’ goes back to the commit id that is mentioned and all the commits after that are erased.
</pre>

![Git Revert and Reset](https://github.com/scpowar/Fraud-Detection/blob/master/git-revert-reset.png?raw=true)