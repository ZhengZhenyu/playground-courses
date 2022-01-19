上一步中介绍的`git pull`命令其实是另外两个命令的结合
`git fetch`及`git merge`。`git fetch`命令从远端拉取
最新代码并创建一个新的分支: remotes/<remote-name>/<remote-branch-name>。这个分支可以使用`git checkout`命令
进行切换。

使用`git fetch`命令可以很好的帮助你在不影响当前分支的情况下
对代码和修改进行检视。使用下面的命令可以将Fetch得到的代码分支
合并到main/master分支
`git merge remotes/<remote-name>/<remote-branch-name> main` 更多有关Merge的内容将会在接下来的内容中介绍。

## 任务

拉取最新的代码修改并切换到该分支以便进行代码检视
`git fetch`
`git checkout remotes/origin/master`

## Tips

可以使用`git branch`查看本地所有的分支，使用
`git branch -r`查看远端所有的分支。
