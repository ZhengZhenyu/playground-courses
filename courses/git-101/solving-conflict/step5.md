有时为了保证仓库中提交记录的间接，项目的维护者会要求将相关的多次提交合并到一次提交中，
使用`git rebase`命令可以很好的完成这个工作。

## 任务

依次执行下面的命令完成准备工作：

1. 切换回`master`分支：
    <pre><code exec="git checkout master">git checkout master</code></pre>

2. 创建并切换到一个新的分支，准备进行接下来的操作：
    <pre><code exec="git checkout -b new_branch_2">git checkout -b new_branch_2</code></pre>

3. 创建新文件 `file1` 并提交：
    <pre>
    <code exec="echo 'This is new_file1' > new_file1">echo 'This is new_file1' > new_file1</code>
    <code exec="git add .">git add .</code>
    <code exec="git commit -m 'Added new_file1'">git commit -m 'Added new_file1'</code>
    </pre>

4. 创建新文件 `file2` 并提交：
    <pre>
    <code exec="echo 'This is new_file2' > new_file2">echo 'This is new_file2' > new_file2</code>
    <code exec="git add .">git add .</code>
    <code exec="git commit -m 'Added new_file2'">git commit -m 'Added new_file2'</code>
    </pre>

5. 使用<code exec="git log">git log</code>查看提交历史，可以看到产生了两次提交；
6. 对于一些项目，维护者要求相关的commit需要合并到一个commit后再提交到上游仓库，使用下面的命令将最近的两次commit进行合并：
    <code exec="git rebase -i HEAD~2">git rebase -i HEAD~2</code>
在弹出的编辑器中进行编辑修改为`pick xxx` `s`

## Tips

`rebase` 时可以通过命令选择多种操作方式，可以根据实际需求进行选择，如图：

![avatar](../assets/rebase.bmp)