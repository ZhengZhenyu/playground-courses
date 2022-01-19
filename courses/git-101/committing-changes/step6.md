上一步中所介绍的`git log`命令仅展示了提交的作者以及commit message信息，
想要查看该提交修改了哪些文件，可以使用`git show`命令。

与先前介绍的许多命令一样，默认情况下`git show`与`HEAD`提交
进行对比，使用`git show <commit-hash>`来指定想要对比的提交。