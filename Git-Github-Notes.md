# Using Git & Github example

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

#### Working with branches

<pre>

git branch' command will show you —
The list of branches in your repository and the branch you are on. (The HEAD will point to the branch you are currently on.)

git checkout -b model <i>#to create a new branch</i>
</pre>

##### Pull and merge 
<pre>
To merge it to the main branch, we used the github UI to create the pull request. 

Pull request means to request the merger of branches. In our case, there were no conflicts and the status was shown as ‘able to merge’. 

 

Conflicts arise when you have different codes in the same file in different branches. Once the pull request was created, we went to the pull request tabs and merged the two branches. 
</pre>

##### Checkout
<pre>
checkout command can be used to switch branches. The syntax to switch to another branch is given as follows:

git checkout #destination-branch-name
 

The command given in this option follows the syntax given above and will switch from the current branch to an existing branch named 'feature'. Hence, this option is the correct choice.
</pre>