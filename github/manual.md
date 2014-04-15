User guide for github
=====================

### Directory

* Working Directory(where you real program locates)

* Stage(Index): A temporary directory saves files to push

* Repository: Directory at github.com

Files flow: Working directory-->Stage-->Repository

### Fundamental commands

* git add files: add file to **Stage**

* git commit: take a snapshort of __Stage__ and commit to **History**

* git reset -- files or git reset: revoke (all)files in **Stage**

* git checkout -- files: cp files from __Stage__ to **Working
  Directory**, overwriten local files

Enter into interactive mode wit **-p**

* git commit -a: Add all files in current directory to **Stage** and
  commit

* TODO: git commit files: Contains last commit and commit of current working
  directory's file's snapshort, files are added to **Stage**

* TODO: git checkout HEAD -- files: rollback to last commit

## Command Detail

### Diff

* `git diff`  --> same as `git diff Stage(add only) Workding_directory`

* `git diff --cached`  --> same as `git diff History(Last_commit) Stage(uncommit)`

    commit(use snapshort to generate commit ID)->History

    push->use commit ID to push source to github.com

* `git diff HEAD`  --> same as `git diff Last_commit(History) Working_directory`

* `git diff parent_branch new_branch` --> commit ID or branch name OK

* `git diff branch_name`  --> same as `git diff branch_name working_directory`

### Commit

* git commit

* git commit --amend -->use the same parent point of current commit to 
commit, old commit will be canceled

### Checkout

* git checkout HEAD~ test.c	# copy commit point(current commit 
point's parent point) file to working directory and stage

* git checkout e

### Checkout

* git tag -l

show remote tags

* git show

chenges in hirtory

* git checkout -b new_branch_name remote_branch_name(tag name)

* git reset --hard HEAD~3	# change current branch to HEAD~3(working directory included)

### Manipulate Branches

* git branch  --> List all branches

* git branch <branch>  --> Create new branch, reference the same point in history

* git branch <branch> <start-point>  --> Create new branch, reference start-point, which may be banch name or tag name

* git branch -d <branch>  --> delete branch, if not reachable from current branch, fail.

* git branch -D <branch> --> force delete branch, if branch points to a commit reachable from other branch or tag

* git checkout <branch>  --> use current branch(branch) to update working directory

* git checkout -b <new> <start-point>  --> create new branch <new> referencing <start-point> and check it out

cat .git/HEAD	--> tell which branch is current


