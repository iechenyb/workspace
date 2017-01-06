# workspace
1. git status（查看本地分支文件信息，确保更新时不产生冲突）
2. git checkout -- [file name] （若文件有修改，可以还原到最初状态; 若文件需要更新到服务器上，应该先merge到服务器，再更新到本地）
3. git branch（查看当前分支情况）
4. git checkout [remote branch](若分支为本地分支，则需切换到服务器的远程分支)
5. git pull  本地未更新最新版本并且做了修改，pull时会有冲突，内容会合并。
若命令执行成功，则更新代码成功！
如果希望保留生产服务器上所做的改动,仅仅并入新配置项, 处理方法如下:
git stash
git pull
git stash pop
git mergetool 直接合并到远端服务器上
