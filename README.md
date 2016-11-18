# Git basic commands
Here list out some basic Git commands to get you going with Git

### 1: Clone - Check out a repository

Create a working copy of a local repository

```html
git clone /path/to/repository
```


### 2: Add files

Add one or more files to branch

```html
git add <filename>
git add *
```

### 3: Commit - Commit changes to head
Commit the files you've added with git add.

* Commit message should be write in release note
* Better using lowercase
* Avoid symbols + - /

```html
git commit -m "Commit message"
```

### 4: Pull - Get update from server or master

Fetch and merge changes on the remote server to your working directory.

```html
git pull origin master/branch
```

### 5: Push - Send changes to branch

Send the changes to the master branch or Other from your local repository

```html
git push origin master/branch
```

**Push all branches** to your remote repository
```html
git push --all origin
```

### 6: Status - List the files you've changed

List the files you've changed and those you still need to add or commit

```html
git status
```

### 7: Branches

**Branch list** - List all the branches
```html
git branch
```

**Add Branch** - Create a new branch and switch to it
```html
git checkout -b <branchname>
```

**Switch Branch** - Switch from one branch to another
```html
git checkout <branchname>
```

**Delete Branch** - Delete the feature branch
```html
git branch -d <branchname>
```

### 7: Log -  Lists the commits

Git log list the commits made in that repository in reverse chronological order

```html
$ git log
```

### 8: Changing a commit message

You can change the most recent commit message using the below command

```html
git commit --amend
```
* The commit only exists in your local repository and has not been pushed to GitHub
* Enter the new commit message and press Enter
* The new commit and message will appear on GitHub the next time you push


### 9: Reset - Revert git repository

To revert to a previous commit, ignoring any changes
* **HEAD** code get from the git log, Use the first eight digit letter from the commit line
* **0d1d7fc3**2e5a947fbd92ee598033d85bfc445a50
* The chamges will appear on GitHub the next time you push

```html
git reset --hard HEAD
git reset --hard 0d1d7fc3
```


### 10: Stash

Now you want to switch branches, but you don’t want to commit what you’ve been working on yet, so you’ll stash the changes.
To push a new stash onto your stack, run git stash

**Stash** - Takes the current state of the working directory and index, puts it on a stack for later

```html
git stash
```

**Stash list** - This command will display a queue of current stash items

```html
git stash list
```

**Stash apply** - If you want to apply one of the older stashes, you can specify it by naming it

```html
git stash apply
git stash apply --index
```
