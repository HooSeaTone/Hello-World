# Hello-World
For Github  Learning

Hi, guys!

Here are some common commands as below.
Just for a reference to myself later days.
(from https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)
(廖雪峰的Git教程)




总结： 常用命令简化如下：

git status

git add -A

git status

git commit -m "Comments to the Changes this time"

git status

克隆远程到本地，修改后上传

git clone git@github.com:HooSeaTone/Hello-World.git

git push -u origin master   （git push origin master)

本地关联远程的github空的repository，并上传

git remote add origin "remote repository URL"

git remote -v

git push origin master

git鼓励大量使用分支：

查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>

