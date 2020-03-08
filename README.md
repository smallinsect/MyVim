# MyVim
xftp

vim编辑软件
启动时是normal

按i 进入编辑状态 按esc退出编辑状态
按a 在光标前插入
按x 删除光标处的字符

方向移动hjkl

按:wq 保存并退出 w存盘 q退出
:x 只有改变 才存盘 退出
ZZ 必要时 才存盘

o在当前行后插入一个新行
O在当前行钱插入一个新行

^行头 $行尾

找文字 normal模式 /endl 查找endl字符串
按n 查找下一个endl字符串

交换两行 ddp dd是删除的意思 并且保存起来 p是粘贴的意思

yyp yy就是复制光标的行 p粘贴

撤销快捷键 u
取消上一次撤销的 ctrl+r

:set hlight

.点号 重复上一个命令
x删除一个字符

删除4行 先敲4 再按dd

显示行
:set number

跳到17行 17G 或者:17
跳到20行 20G 或者:20
跳到文件第一行 gg
跳到文件最后一行 G

W跳过一个单词
e跳到词尾

%跳到下一个匹配符号

/*是下一个 #是上一个 

v 进入virtual模式，可以移动光标选择范围，运行命令是针对选项范围
shift+v 移动光标直接 选中

th到一个字符的前一个位置

快速注释
块模式ctrl+v 光标向下移动
再按I进入插入模式 按//
再按esc
被块模式下的行都会被注释

vim补全
ctrl+n和ctrl+p
vim代码格式
选中按=号

J把所有的行连接起来
j把一行边多行

横向分屏 :split 纵向分屏 :vsplit
切换屏幕编辑 ctrl+w+w
隐藏分屏 :hide

vim使用教程 vimtutor

虚拟机服务器之间拷文件
scp usmall@192.168.79.140:/home/a.cpp .
将这个服务器的文件拷贝到本机上

基础配置wim
第一种 找到配置文件 vim etc/vim/vimrc
第二种 找到配置文件 vim usr/share/vim/vimrc
配置如下
set autoindent     ""自动缩进
set cindent        ""以C语言的方式缩进
set shiftwidth=4   ""设置自动缩进的空格数量
set softtabstop=4  ""tab键的实际占有空格数，统一缩进
set tabstop=4      ""设置tab键的空格数

:set tabstop=4 设定tab宽度为4个字符
:set shiftwidth=4 设定自动缩进为4个字符
:set expandtab 用space替代tab的输入
:set noexpandtab 不用space替代tab的输入

快速选中并复制粘贴替换一个单词
1.光标移动到aaa的开头，按 v 按e 按y
2.光标移动到bbb的开头，按 v 按e 按p
也就说，快速选中一个单词，按v按e即可。

