
1.  Can we have a global.gitignore?
=>  Yes, we can create a global.gitignore file. For example, if we don't want to push certain files in 
    your Github, we can save it inside the .gitignore_global folder created. These folders will be available in the local data but it will not be pushed.


2.  How to find the difference between two commits?





3.  Write difference between git and git commit commands. 
=>  git is the main command for interacting with Git. We can do variety of operations with it, like creating,     
    adding files, committing changes, and pushing changes, to a remote repository by using a variety of the subcommands. 

    The git commit command helps us update the local repository. The git commit command creates a new commit that has all the changes, insertion and deletion made since the last commit. To make it simpler for others to understand the changes you have made, it is advisable to add a concise and clear explanation in the commit message.


4.  How to unstage files?
=>  After working directory, by using git add . command we reach to staging area which later we commit to 
    Git repository. In order to unstage the staged file, we can use various commands to unstage it like: 
    For example, to unstage a file named myfile.txt, run the following command:
    
    git reset "filename.txt" OR git restore --staged "filename.txt" 
    
    This will remove the file from the staging area, but the changes will still be present in the local directory.


5.  How to revert a commit?
=>  A new commit is required that undoes the changes made in the initial commit to revert a commit.
    We can do it by using git log--oneline to get SHA code for our file and use 

    git revert "The SHA CODE" 

    
6.  Difference between revert and reset. 
=>  These commands are used to undo changes in git. 
    git reset basically means to undo the local changes to the state of GIT repository. We can recover a deleted file after using reset whereas git revert undo's an entire commit from way back. Revert command creates a new commit in order to undo changes made by some other commits.