# 06 Linux 命令行使用

## 1 命令行介绍

命令提示符是在操作系统中，提示进行命令输入的一种工作提示符。

在不同的操作系统环境下，命令提示符各不相同。

* windows： 命令行程序为cmd.exe，是一个32位的命令行程序，微软Windows系统基于Windows上的命令解释程序，类似于微软的DOS操作系统。windows系统的命令脚本为bat脚本。
* Linux：终端控制台，Linux系统的命令脚本为shell脚本。

一般说的“命令行”是指linux命令，linux命令是对Linux系统进行管理的命令。

对于Linux系统来说，无论是中央处理器、内存、磁盘驱动器、键盘、鼠标，还是用户等都是文件，Linux号称一切皆是文件。Linux系统管理的命令是它正常运行的核心，与之前的DOS命令类似。

Linux命令在系统中有两种类型：

* 内置Shell命令
* Linux命令

## 2 **帮助文档**

* man：Linux下的帮助指令，通过man指令可以查看Linux中的指令帮助、配置文件帮助和编程帮助等信息。
* info：Linux下info格式的帮助指令。就内容来说，info页面比man page编写得要更好、更容易理解，也更友好，但man page使用起来确实要更容易得多。
* help：用于显示shell内部命令的帮助信息。help命令只能显示shell内部的命令帮助信息。而对于外部命令的帮助信息只能使用man或者info命令查看。

## 3 键盘和光标

### 3.1 **tab补全**

- `Tab` 补全是非常有用的一个功能，可以用来自动补全命令或文件名，省时准确。
- 未输入状态下连按两次 `Tab` 列出所有可用命令
- 已输入部分命令名或文件名，按 `Tab` 进行自动补全，多用你就肯定会喜欢的了。

### 3.2 **光标**

* up 方向键上（可以调出输入历史执行记录，快速执行命令）
* down 方向键下（配合 up 选择历史执行记录）
* Home 移动光标到本行开头
* End 移动光标到本行结尾
* PgUp 向上翻页
* PaDN 向下翻页
* Ctrl + C 终止当前程序
* Ctrl + L 清屏 = clear命令（记住这个快捷键，比clear高效很多）

## 4 **绝对路径和相对路径**

* 绝对路径（absolute path）：由根目录(/)开始写起的文件名或目录名称， 例如 /root/.bashrc；
* 相对路径（relative path）：相对于当前路径的文件名写法，即以当前所在路径的相对位置来表示。 例如 ./root/.bashrc 或 http://www.baidu.com/ 等等，简单来说，开头不是 / 就属于相对路径的写法。

**特殊目录**

| 符号 | 含义                                              | 备注 |
| ---- | ------------------------------------------------- | ---- |
| .    | 代表当前的目录，也可以使用 ./ 来表示              |      |
| ..   | 代表上一层目录，也可以 ../ 来代表                 |      |
| ~    | HOME目录，`cd ~` 与 `cd $HOME` 和 `cd` 的效果一样 |      |
