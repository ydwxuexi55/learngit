


   git 简注
   git init  把当前目录变成Git可管理的库
   
   把一个文件放进Git仓库只要进行两部
   1   git add 文件名
   2   git commit -m "注释"

   git status
   获取Git仓库当前状态（文件有无被修改）  modified
   git diff 文件名
   查看文件difference
   git log 
   显示最近到最远的提交日志
   git log --pretty=online
   简化显示信息
   git reset --hard HEAD^
   回退倒上一版本
   git reset --hard HEAD^^
   回退倒上上一版本
   git reset --hard HEAD~100
   回退倒往上100个版本
   git reset --hard <commit id>
   指定返回某一版本文件
   git checkout --file
   丢弃工作区的修改（文件内容改乱，直接丢弃工作区的修改）
   git reset HEAD <filename>
   将暂存区的修改撤销掉
   git rm <filename>
   从版本库中删除文件
   
   远程连接

   git remote add origin git@github.com:xxx
   添加远程库
   git push origin master
   发送文件给远程库
   git clone git@github.com:xxx


   创建与合并分支
   一开始的时候   HEAD  -->  master分支  -->最新的提交（commit）
   创建dev分支  性价一个dev指针   
   git branch dev
   创建dev分支
   git checkout dev 
   切换到dev分支
   git checkout -b dev
   简化  创建并切换dev分支
   git branch
   查看分支（当前分支前有*号）
   git merge dev
   合并dev到master上（切换到master上）
   git switch dev
   切换到dev分支
   git switch -c <name>
   创建分支并切换
   git branch -d <name>
   删除分支