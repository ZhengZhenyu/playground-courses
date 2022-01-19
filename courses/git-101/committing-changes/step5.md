通过`git log`命令可以查看当前仓库的所有提交的历史纪录。

## Tips

log命令的输出格式非常灵活，可以通过相应的参数进行指定。
例如想要在每一行中输出一条提交记录，可以使用如下命令：
`git log --pretty=format:"%h %an %ar - %s"`
更多内容可以参考`git log --help`
