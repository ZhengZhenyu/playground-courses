一旦修改被添加到准备区域(Staged Area)，在使用`git diff`时，
将不会再包含这些修改。因为默认情况下`git diff`只对比工作目录
(Working Directory)之间的差异。

若想对比准备空间(Staging Area)与历史版本之间的差异，需要指定
相应的参数：`git diff --staged`。