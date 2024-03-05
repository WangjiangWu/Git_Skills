# Git_Skills

# create a new repository on the command line
- echo "# ***" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin {ssh key}
- git push -u origin main


# push an existing repository from the command line
- git remote add origin {ssh key}
- git branch -M main
- git push -u origin main


# other codes:
- git branch
- git status


- git config --list
- git config -e [--global]
- git config --global user.name "***"
- git config --global user.email "***"
- git status
- git diff filename
- git log  (git log --pretty=oneline)
- git reset --hard HEAD^ (HEAD^^) or (git reset --hard HEAD~100) or (git reflog, git reset --hard ID)
- git checkouot -- <file>
- git rm filename, git checkout --<filename>


# Remote
- SSH Key (id_rsa, id_rsa.pub)
- ssh-keygen -t rsa -C "youremail@example.com"
- git clone <github link>


- git checkout -b <dev> (git branch <dev>, git checkout dev)
- git branch
- git checkout <branchName> 
- git merge dev
- git branch -d dev

- git merge --no-ff -m "message"
- git stash
- git stash list
- git stash apply (git stash drop) or git stash pop


- git remote (git remote -v)
- git checkout -b dev origin/dev
- git pull
- git branch --set-upstream dev origin/dev

Ref:
https://zhuanlan.zhihu.com/p/30044692
https://www.liaoxuefeng.com/wiki/896043488029600/900003767775424