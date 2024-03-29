Repository initialization and configuration.

 # initialize the repo.
 git init
 
 # add the remote origin of the repo.
 git remote add origin https://github.com/user/repo.git
 
 # verify remote origin.
 git remote -v
 origin  https://github.com/user/repo.git (fetch)
 origin  https://github.com/user/repo.git (push)
Set-up email and user name.

 git config user.email "juan_dela_cruz@example.com"
 git config user.name "Juan Dela Cruz"
Check status of all files in the repository

 git status
Adding untracked files or delete files.

 # add a file to track.
 git add file_name.any

 # add all files.
 git add -A
Commiting and pushing changes and added files.

 # commit all changes.
 git commit -am "My commit message"

 # push to a branch.
 git push origin master
Pulling and merging changes from a branch.

 # pull any updates from a branch.
 git pull origin master
 
 # In the case of unrelated histories add --allow-unrelated-histories
 git pull origin master --allow-unrelated-histories
 
 # all changes will be merged and will notify for merge conflicts. 
 # if there are conflicts then resolve them manually.
 # commit and push the changes to a branch.
 git push origin master
Cloning a repository.

 git clone https://github.com/user/repo.git
 # example
 git clone https://github.com/arielmagbanua/android-mobile-app-dev-examples.git
Git Branching Guides
Creating a branch.

 git checkout -b branch_name
Checkout a branch.

 git checkout branch_name
Merging updates from other branches.

 # merge changes from example_branch_name_1
 git merge example_branch_name_1
 
 # in case of unrelated histories add --allow-unrelated-histories
 git merge example_branch_name_1 --allow-unrelated-histories
 
 # after merging if there are merge conflicts manually resolved them.
 # commit the branch.
