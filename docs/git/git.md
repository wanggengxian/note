## 命令
|command|comments|
|---|---|
|git push origin --delete [branch-name]|删除远程分支|
|git checkout -b [local-branch] origin/[remote-branch]|检出远程的remote-branch分支到本地|
|git push origin [local-branch]:[remote-branch]|推送本地的local-branch(冒号前面的)分支到远程origin的remote-branch(冒号后面的)分支(没有会自动创建)|
|git branch -d [local-branch]|删除本地分支|