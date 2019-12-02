


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
丢弃工作区的修改


