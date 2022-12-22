Working Directory > Stage > Local Repository > Remote

Two ways to initialize a git repository:
git init - initialize a git repository in your local machine
git clone - to clone a git repository from github

Commands to add files and folders to the staging phase:
 git status - to check what changes happened to a git repo
 git add --all / git add -A  - add all new and changed files to the staging area (current directory + root directory > if executed from a child directory)
git reset - unstage new and changed files
git reset --hard - unstage and get back deleted files to the working directory
 git add . - add all new and changed files in the current directory 
git add * - add all new and changed files to the stage except the deleted one
git add one.txt - add only one file to the staging
git add *.txt - add all new and modified files(no folders, no deleted files) only in the current directory
git rm one.txt - deletes the file and adds to the staging area
git rm one.txt -f - to delete forcefully after modification of file and adds to staging.
git rm one.txt --cached - keep the file but changes added to staging.

Commands to commit after staging:
git commit -m “message what changes happened” - commit command
git reset HEAD~ - to go back to unstaged condition after commiting

Branching in git & github:
git branch - print the total number of branch
git branch branch_name - create a new branch by taking everything from main branch
git checkout branch_name - switch to a different branch
git merge branch_name_to_merge_with -m “message of merging” - merge two branch

Push to a remote repository which is github in my case:
git push origin main - here origin is the remote repository and main is the main branch of remote repository
git push origin branch_name - here branch_name branch will be created in remote repository and you can push from branch_name.

Get source code from remote origin:
git fetch - take changes made in remote origin
git merge - change that is made in remote origin reflect in local repository
git pull = git fetch + git merge
