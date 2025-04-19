1. `git init` -> Powers your folder to be managed by git, and initialises a new empty repository. It also creates a .git folder that has all 
the relevant logic to manage versions of your projects.

2. `Working area` -> There can be a bunch of files that are not currently handled by git.
It means that changes are done are to be done are not managed by git yet. a file which is in working area is considered to be not in
staging area. 
When we do `git status` and we see a bunch of `untracked files` than these are actually called to be working area.

3. `Stage Area` -> What all files are going to be part of the next version that we will create, This staging area is the place where git knows what changes will be done from the last version 
to next version.

Command:- `git add .`

Now if we want to remove this file from staging area we need to use Command

`git rm --cached README.txt`

4. `Repository area` -> This area actually contains the details of all your prev registerd version. And the files in this area, git
already manages them and knows their version history.



5. `git add <file>` -> This moves file from working area to staging area.

6. `git rm --cached <file>` -> Moves file back from staging area to working area.

7. `commit` -> Commit is a particular version of the project. It captures a snapshot of the project's staged changes and created a version out of it.

8. `git commit` - Registers staging changes to a commit.


9. `git log` -> will show all the commit history.

10. `git restore <file>` -> It removes all files changes from the staging area to be commited. This can be useful, if we did some dirty piece of code and 
now no more want it. Instead of deleting every changes line by line, we can restore it or you can say restore last clean version of the file.

11. `git restore --staged <file>` -> It removes file from stageing area to working area.

12. Difference between git rm and git restore
ans: If you want to move the whole file back to the untracked state, then we do git rm, otherwise if we just want the changes to be moved in working area 
or staging the we do git restore.

