# Hello-World
For Github  Learning

Hi, guys!

Here are some common commands as below.
Just for a reference to myself later days.
(from https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)
(廖雪峰的Git教程)

$ git config --global user.name "MyUserName"

$ git config --global user.emai "MyEmail"

$ mkdir myproject

$ cd myproject

$ pwd

$ git init    (initializing the working directory)

$ ls -ah      (list files)

$ git add “filename”
  
$ git commit -m "Comments to the Changes this time"

$ git status   (to observe the status at present)

$ git checkout -- “filename”    (not including the specified file)
  
$ git diff “filename”
  
$ git log

$ git log --pretty=oneline

$ git reset --hard HEAD^  (or HEAD-100, or version-hash, no need to a complete hash.)

$ cat “filename”
  
$ git reflog

场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。

场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD <file>，就回到了场景1，第二步按场景1操作。

场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。git reset --hard HEAD^  (or HEAD-100)
  

要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；


总结： 常用命令简化如下：
git status
git add -A
git status
git commit -m "Comments to the Changes this time"
git status
