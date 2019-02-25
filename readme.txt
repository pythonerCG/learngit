Git is a distributed version control system.
Git is free software distributed under the GPL

git init  --- 初始化文件为本地仓库
git add filename  --- 上传文件
git commit -m '操作描述'  --- 描述此次操作所做的修改与变更
git status  ---  时刻掌握仓库当前的状态（谁被修改，）
git diff filename  --- 查看修改前后的不同difference
git log  (--pretty=oneline)  --- 显示从最近到最远提交的日志
git reset --hard HEAD^  --- 恢复到上一版本
git reset --hard commit_id  --- 恢复到指定版本
git reflog  --- 用来记录每次命令
