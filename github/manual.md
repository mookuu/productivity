Github's manual-simple version
==============================

## Remote Setting


### Create pository

* Login github and New repository


## Local Setting

### Generate ssh key and add to github

1. $ssh-keygen -C 'email address' -t rsa

2. add ssh key(~/.ssh/id_rsa.pub) to github.com(setting->ssh key)

3. test link to github. `ssh -v git@github.com`

### Install git

* $sudo apt-get install git

### Git user setting

1. $git config --global user.name "name"

2. $git config --global user.email email

### Create local workspace

* mkdir repository

* git init && ls -al

### Add remote repository

* $git remote add origin git@github.com:takechiyocn/apue.git

* git remote

### Add file(s), commit and push

* $git add file(s)

* $git commit -m "comment"

* $git push origin master
