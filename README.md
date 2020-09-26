## ......A Basic Overview of Git Commands......

![git photo](https://user-images.githubusercontent.com/68290275/93714505-c3f1a280-fb80-11ea-80b1-fed31d8ef150.png)

### 1: git config
- **git config --global user.name “name”**
- **git config --global user.email “email”**

 These commands set the author name and email address respectively to your git. With these commands you
 tell the git who you are.
- **git config --global --list**

 This command is used to check the git configuration (user name and email).

### 2: git --version
 This command is used to check the version of git.

### 3: git command --help (e.g. git config --global --help)
 This command is used to get help about the related command.
 
### 4: git init
 This command is used to Initialize a local Git repository. With this command you are transforming the 
 current directory into a Git repository (now the git will have access over it).
 
### 5: rm –rf .git
 This command is used to undo git init. To uninitialize a git repository, you simply need to remove the 
 folder named ".git" in your repository folder. This can be done by manually deleting the folder or by 
 using the given command (rm -rf .git) in terminal.
 
### 6: git status
 This command returns the current state of the repository.
 
### 7: git add
 This command adds a file to the staging area.  It tells Git that you want to include updates to a 
 particular file in the next commit. However, changes are not actually recorded until you run git commit.
 
- To add a particular file, use the following command: **git add fileName**
- To add  all changed files of a particular directory, use the following command from that directory: **git add .**
- To add changed files of entire working tree, use the following command from any where in that tree: **git add -A**
- To add files (modified and deleted) except untracked files of entire working tree, use the following command: **git add –u**

### 8a: git reset
 This command unstages all the files( moves them back from staging area to working directory.), but it
 preserves the file contents. 
- 8b: **git reset fileName**: This command unstages only one file.
- 8c: **git rm --cached fileName**: This command can also be used for unstaging the file.

### 9: git diff
 The git diff command allows us to track the changes that are staged but not committed.
 
### 10: git commit –m ‘message’
 The "commit" command is used to save the changes to the local repository. Git commit is like setting 
 a checkpoint in the development process which you can go back to later if needed.We also need to write 
 a short message to explain what we have developed or changed in the source code.
- **Git commit –m ‘message’ fileName**: This command is used to commit the given particular file.
- **Git commit --amend –m ‘message’** :This command is used to fix the commit message. In case the 
 commit message is typed wrong this command can be used to rewrite the commit.

### 11: git log 
 The git log command displays all of the commits in a repository’s history.
 By default, the command displays each commit’s: Secure Hash Algorithm, author, date and commit message.

### 12: git branch
The git branch command is used for creating, listing and deleting branches.
- **git branch**: This command shows all the local branches in the current repository (also shows on 
 which branch are you currently).
- **git branch branchName**: This command is used to create a new branch.
- **git branch -d branchName**: This command is used to delete the branch.
- **git checkout branchName**: This command is used to switch from one branch to another.
- **git checkout –b branchName**: It is a shortcut command that allows you to create and switch to a 
 branch at the same time.
- **git merge branchName**: When the branch is completely developed and everything works fine, the final 
 step is merging (combining) the branch with the parent branch. This command is used for that purpose. It 
 is important to remember that you first need to be on the specific branch that you want to merge with 
 your feature branch.For example, when you want to merge your feature branch into the master branch then 
 first you should switch to the master branch:
		git checkout master
		git merge branch_name

### 13: git remote add origin your_url:
 This command is used to connect your local repository to the remote server.

### 14: git push
 The git push command is used to upload local repository content to a remote repository. Command git 
 push requires two parameters: the remote repository and the branch that the push is for. 
 **git push remoteName branchName** 
 Example: **git push origin master**  where remote name is origin and branch name  is master. 
- **Git push –u remote_name branch_name**: When you use this command then next time you don’t need to 
 write full command for push. At that time git push is used intead of git push –u remote_name branch_name.

### 15: git clone remote_url
 To create a local working copy of an existing remote repository, use git clone to copy and download the 
 repository to a computer. Cloning is the equivalent of git init when working with a remote repository. 
 Git will create a directory locally with all files and repository history.

### 16: git pull remoteName branchName
 To get the latest version of a repository run git pull. This pulls the changes from the remote repository 
 to the local computer. Use git pull to update a local repository from the corresponding remote repository. 

## so start ↴:
![git photo2](https://user-images.githubusercontent.com/68290275/93714533-ebe10600-fb80-11ea-85a4-0fd41f778df0.png)

