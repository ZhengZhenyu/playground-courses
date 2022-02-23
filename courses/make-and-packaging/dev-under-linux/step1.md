在Linux下，软件开发工具通常被切割成一个个独立的小工具，各自处理不同的问题。以C语言软件开发为例，编辑器（emacs， vim等）用来进行编辑程序的，调试器（gdb）用来调试程序，编译器（GCC）用来编译和链接程序的，性能分析工具（gcov， gprof）用来优化程序，文档生成器（doxygen）用来生成文档等等。

本课程中我们将使用最基本的Vim编辑器以及Gcc编译器来演示如何在Linux下进行最基本的软件开发，在正式开始前，我们首先要检查环境中是否有这些软件以及其版本。

## 任务

使用`which`命令来检查所要用到的软件是否在环境中正确安装与配置。

<pre>
<code exec="which gcc">which gcc</code>
<code exec="which vi">which vi</code>
</pre>

使用下面命令来检查所要用到的软件版本是否满足你的开发需求。

<pre>
<code exec="gcc --version">gcc --version</code>
<code exec="vi --version">vi --version</code>
</pre>

进入工作目录进行下一步学习：
<code exec="cd chapter1">cd chapter1</code>