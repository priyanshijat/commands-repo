```
sudo apt update
```
to update the system

```
sudo apt-get install git -y
```
to install git 

```
mkdir (folder-name)
```
create folder 

```
cd (folder-name)
```
enter in folder

```
git init
```
creates a new Git repository

```
git config --global user.name <username>
git config --global user.email <email>
```
to set username and email

```
git status
```
to check the status of files

```
git add (file-name)
```
to add a change in the working directory to the staging area

```
git commit -m (file-name)
```
to save all the changes in git repository

```
git restore --staged <file-name>
git rm --cached <file-name>
```
to unstage file from staging area

```
git commit --amend
```
edit latest commit in staging area

```
git log
git log --oneline
``` 
to check all the logs

```
git branch list
```
to list all the branch


```
git branch (branch-name)
```
to create new branch

```
git checkout (branch-name)
git switch (branch-name)
```
to swith in other branch

```
git checkout -b (branch-name)
```
create and switch in new branch 

```
git branch -m <old-name> <new-name>
```
to change branch name

```
git checkout -d <branch-name>
```
to delete branch (soft deletion)

```
git checkout -D <branch-name>
```
to delete branch (forcefully delete)



```
git merge (branch-name)
```
to merge changes 

```
git clone (repo-url)
```
to download a repo in your local system

```
git fetch (repo-url)
```
git fetch gets the latest updates from the remote, but doesn't change your files.

```
git remote -v
```
shows the remote repositories connected to your local Git repo, along with their URLs.

```
git remote add origin https://<your-username>:<your-PAT>@github.com/<your-username>/<repo-url>
```
to add repo

```
git remote set-url origin https://<your-username>:<your-PAT>@github.com/<your-username>/<repo-url>
```
to set url 

```
git push -u origin <branch-name>
```
to push changes from local to remote

```
git pull <branch-name>
```
to pull changes from remote to local

```
git reset --soft HEAD~1
```
Soft Reset (keeps changes staged).

```
git reset --mixed HEAD~1
```
Mixed Reset (unstages changes but keeps files)

```
git reset --hard HEAD~1
```
Hard Reset (removes all changes).

```
git revert HEAD
```
Revert a commit safely

```
git rebase <branch-name>
```
to rebase

```
git stash
git stash list
git stash pop
git stash apply
git stash clear
```
Stash commad


```
git cherry-pick <commit-hash>
```
use cherry-pick command



