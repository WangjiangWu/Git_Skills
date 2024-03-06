# Git_Skills
Wangjiang WU, @SMU

![image](git_sche.png)

# Tutorial
- git
- git help (or -h) commandName
- git help tutorial
- visual studio code

# git config
- git config --list
- git config -e [--global]
- git config --global user.name "***"
- git config --global user.email "***"

# create a new repository on the command line
- echo "# ***" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin {ssh key}
- git push -u origin main
- git push origin main (git push --force origin main)

# push an existing repository from the command line
- git remote add origin {ssh key}
- git branch -M main
- git push -u origin main

# change file
- git status
- git diff filename
- git log  (git log --pretty=oneline) (git log --graph)
- git reset --hard HEAD^ (HEAD^^) or (git reset --hard HEAD~100) or (git reflog, git reset --hard ID)
- git diff HEAD -- readme.txt
- git checkout --file
- git reset HEAD <file>
- rm filename, git rm filename, git checkout --<filename>

# branch
- git branch
- git checkout -b dev 
- git switch -c dev
- git checkout -b dev origin/dev
- git branch dev
- git checkout dev or git switch dev
- git merge dev (for fast forward mode)
- git merge --no-ff -m "merge with no-ff" dev
- git status
- git log --graph --pretty=oneline --abbrev-commit
- git branch -d (-D) dev
- git rebase

- git branch --set-upstream-to=origin/dev dev
- git pull
- git branch --set-upstream dev origin/dev

- git stash, git status
- git stash list
- git stash apply, git stash drop. or (git stash pop)
- git stash apply stash@{0}
- git cherry-pick 4c805e2

# tage
- git tag -d v0.1 (git push origin:refs/tags/v0.1)
- git push origin v1.0
- git push origin --tags

# Fork
- git clone ...
- pull request

# Remote
- SSH Key (id_rsa, id_rsa.pub)
- ssh-keygen -t rsa -C "youremail@example.com"
- git clone <github link>
- git remote (git remote -v)
- git remote rm filename
- git remote rm origin

# git ignore
- .gitignore
- [git ignore templates] (https://github.com/github/gitignore)
- [gitIgnore Online Generator] (https://michaelliao.github.io/gitignore-online-generator/)

# Ref:
- https://docs.github.com/zh/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
- https://zhuanlan.zhihu.com/p/30044692
- https://www.liaoxuefeng.com/wiki/896043488029600/900003767775424
