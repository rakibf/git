Working Directory > Stage > Local Repository > Remote

>> Two ways to initialize a git repository:
git init - initialize a git repository in your local machine
git clone - to clone a git repository from github

>> Check git status:
git status - to check what changes happened to a git repo

>> Add files & folders to staging
git add --all / git add -A  - add all new or changed files & folders to the staging area (current directory + root directory > if executed from a child directory)
git add . - add all new and changed files & folders in the current directory 
git add * - add all new and changed files & folders to the stage except the deleted one
git add one.txt - add only one file to the staging
git add *.txt - add all new and modified files(no folders, no deleted files) only in the current directory

>> Back to untracked condition after git add
git reset - unstage new and changed files & folders

>> discard all changes after the last commit
git reset --hard - unstage and get back deleted files to the working directory

>> discard commited change and go back to the last commit (be careful)
git revert HEAD

>> git remove
git rm one.txt - deletes the file and adds to the staging area
git rm one.txt -f - to delete forcefully after modification of file and adds to staging.
git rm one.txt --cached - keep the file but changes added to staging.

>> commit after staging:
git commit -m “message what changes happened” - before commit everyone can see your changes but after commit no one can see

>> branching in git & github:
git branch - print the total number of branch and your current branch name
git branch branch_name - create a new branch by taking everything of the branch from where you created the new one
git checkout branch_name - switch to a different branch
git merge branch_name_to_merge_with -m “message of merging” - merge the branch_name_to_merge_with to your current branch

Push to a remote repository which is github in my case:
git push origin main - here origin is the remote repository and main is the main branch of remote repository
git push origin branch_name - here branch_name branch will be created in remote repository and you can push from branch_name.

Get source code from remote origin:
git fetch - take changes made in remote origin
git merge - change that is made in remote origin reflect in local repository
git pull = git fetch + git merge
