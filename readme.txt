Git is a distributed version control system.
Git is free software distributed under the GPL

git init  --- 初始化文件为本地仓库
git add <filenam>e  --- 上传文件
git commit -m '操作描述'  --- 描述此次操作所做的修改与变更
git status  ---  时刻掌握仓库当前的状态（谁被修改，）
git diff <filename>  --- 查看修改前后的不同difference
git log  (--pretty=oneline)  --- 显示从最近到最远提交的日志
git reset --hard HEAD^  --- 恢复到上一版本
git reset --hard commit_id  --- 恢复到指定版本
git reflog  --- 用来记录每次命令
git checkout -- file  撤销修改
   一种是 readme.txt 自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态
   一种是 readme.txt 已经添加到暂存区后，又做了修改，现在，撤销修改就回到添加到暂存区后的状态。
   总之，就是让这个文件回到最近一次git commit 或 git add时的状态
   git checkout -- file 命令中的 -- 很重要， 没有 --，就变成了‘切换到另一个分支’的命令。
git reset HEAD <filename> --可以把暂存区的修改撤销掉，重新放回工作区。
git rm <filename>  -- 删除文件（删除工作区文件后需要git commit）
git remote add origin git@github.com:pythonerCG/learngit.git  -- 把本地仓库的内容推送到GitHub仓库 （远程仓库的名字为origin,这是git默认的叫法）
git push -u origin master -- git push 实际上是把当前分支master推送到远程。
  由于远程库是空的，我们第一次推送master分支时，加上了-u参数。
git push origin master -- 只要本地坐了提交，就可以通过git push origin master 把本地 master分支的最新修改推送至GitHub。
git checkout -b dev -- 创建dev分支，然后切换到dev分支
  git checkout 命令加上-b 参数表示创建并切换，相当于一下两条命令：
    git branch dev
    git checkout dev
git branch  -- 查看当前分支（当前分值会标一个*号）
git merge + 分支名称  -- 用于合并指定分支到当前分支。
git branch -d +分支名称  -- 删除分支 
