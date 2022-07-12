# hellogit
hello-github
Hi I am sam nice to meet you.




任意一个文件夹内运行初始化一个空库
git init

创建一个分支 名字叫main
git branch -M main

与远程的库关联起来，本地叫origin
git remote add origin git@github.com:samwu-design/nv_back_propagation.git

增加说明文件
git add README.md

提交
git commit -m "first commit"

上传数据，本地origin内容传到远程库的master分支
git push -u origin master




删除误上传的大文件
 git filter-branch --force --index-filter "git rm --cached --ignore-unmatch  路劲/大文件" --prune-empty --tag-name-filter cat -- --all

                                         


配置个人信息
git config --global user.name  "samwu-design"
git config --global user.email  "wusha_1111@163.com"


查看配置个人信息
git config --global --list
删除配置
git config --global --unset (等号前面的字符)


查看日志
git log
git log --oneline  简洁版

---------版本管理----------------------------------------------
版本回退
回退到上一次提交版本
git reset --hard Head~0
   
回退到上上一次提交版本
git reset --hard Head~1  

精确回退到某一个版本，通过log开源查看到
git reset --hard '版本号'
git reflog


分支默认是master
创建分支
git branch 'dev'
切换分支
git checkout 'dev'

合并分支，把当前分支与dev分支合并
手动处理冲突，再提交一次
git merge 'dev'


---------本地与gihub---------------------------------------
注册登录
新建自己仓库respostory
https://github.com/samwu-design/BackTran.git







