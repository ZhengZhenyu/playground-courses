命令`git diff`{{execute}}可以帮助你在当前的工作目录(Working Directory)
与之前的某一次提交的版本之间进行对比，默认情况下将与
`HEAD`提交之间进行对比。

如果你想与更老的版本进行对比，那么可以使用`git diff <commit-id>'
来与指定的提交进行对比。`git diff`的输出时当前工作目录
与历史版本之间所有差异的内容。如果你只想查看某个文件的差异
可以通过指定文件名来进行对比，如：`git diff committed.txt`

## Tips
默认情况下`git diff`的输出格式是合并显示(Combined Diff Format)
可以通过`git difftool`来加载更多显示模式工具。