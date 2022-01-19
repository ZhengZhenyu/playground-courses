当一个文件被添加到准备区域(Staging Area)后，它就可以被提交(Commit)
到仓库(Repository)中了，`git commit -m "commit message"`命令可以
将文件从准备区域移动到仓库并且记录必要的信息，例如提交时间、作者以及
对该提交进行说明的提交描述(Commit Message)。

只有被添加到了准备区域(Staging Area)的修改才能被提交到仓库中，任何在
工作目录(Working Directory)中被修改了但是尚未添加到准备区域中的文件
不会被提交。

## 任务

通过`git commit -m "<commit message>"`{{execute}}命令来将准备区域中的
修改提交到仓库中。

## Tips

每一个提交(Commit)都会被赋予一个`SHA-1`哈希值，以便用户使用其他命令来对其
进行检索
