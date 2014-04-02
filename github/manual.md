User guide for github
=====================

### Directory

* Working Directory(where you real program locates)

* Stage(Index): A temporary directory saves files to push

* Repository: Directory at github.com

Files flow: Working directory-->Stage-->Repository

### Fundamental commands

* git add files: add file to **Stage**

* git commit: take a snapshort of __Stage__ and commit(to **History**)

* git reset -- files or git reset: revoke files in **Stage**

* git checkout -- files: cp files from __Stage__ to **Working
  Directory**, overwriten local files

Enter into interactive mode wit **-p**

* git commit -a: Add all files in current directory to **Stage** and
  commit

* TODO: git commit files: Last commit add snapshort of working
  directory file's commit, files are added to **Stage**

* TODO: git checkout HEAD -- files: rollback to last commit

## Command Detail

### Diff

* `git diff`  --> same as `git diff Stage(commit OK) Workding_directory`

* `git diff --cached`  --> same as `git diff Last_commit(History) Stage(uncommit)`
  commit(snapshort generate commit ID)->History
  push->use commit ID to push source to github.com

* `git diff HEAD`  --> same as `git diff Last_commit(History) Working_directory`

* `git diff parent_branch new_branch` --> commit ID
  `git diff branches1 branches2` --> branch name OK

* `git diff branch_name`  --> same as `git diff branch_name working_directory`
