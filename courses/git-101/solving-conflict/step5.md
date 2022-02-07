有时为了保证仓库中提交记录的间接，项目的维护者会要求将相关的多次提交合并到一次提交中，
使用`git rebase`命令可以很好的完成这个工作。

## 任务

依次执行下面的命令完成准备工作：

1. 切换回`master`分支：
    `git checkout master`

2. 创建并切换到一个新的分支，准备进行接下来的操作：
    `git checkout -b new_branch_2`

3. 创建新文件 `file1` 并提交：
    `echo 'This is file1' > file1`
    `git add .`
    `git commit -m 'Added File1'`

4. 创建新文件 `file2` 并提交：
    `echo 'This is file2' > file2`
    `git add .`
    `git commit -m 'Added File2'`

5. 使用`git log`查看提交历史，可以看到产生了两次提交；
6. 对于一些项目，维护者要求相关的commit需要合并到一个commit后再提交到上游仓库，使用下面的命令将最近的两次commit进行合并：
    `git rebase -i HEAD~2`
在弹出的编辑器中进行编辑修改为`pick xxx` `s`
