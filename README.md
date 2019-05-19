# Jetbrain软件的一些常用功能总结

使用PhpStorm进行搬砖快到一年了，今天闲来无事看看phpstorm的一些功能，感觉不看真的会后悔一辈子，太多太多好用的快捷键和功能了

## 快捷键

#### 编辑
+ `ctrl` + `/` 什么?你竟然不知道这样注释?
+ `ctrl` + `enter` 在行中进行向下换行
+ `ctrl` + `l` 选中本行
+ `ctrl` + `[]` 选中一些行进行缩进
+ `ctrl` + `j` 下一行退格到本行，选中多行则缩成一行
+ `ctrl` + `shift` + `l` 代码格式化
+ `ctrl` + `shift` + `↑↓` 单行代码向上替换位置
+ `ctrl` + `shift` + `v` 查看复制板的历史
+ `ctrl` + `shift`+`enter` 在行中进行向上换行 当选中函数的时候，将函数移到下个函数后；当选中代码的时候，将代码向上移动
+ `ctrl` + `alt` + `z` 选中行则此行恢复到上一个commit，否则恢复整个文件到上一个commit
+ `alt` + `t` 用for/foreach/try...catch等进行包裹
+ `alt` + `l` 不断扩大搜索范围(从变量到行到函数到类)
+ `shift` + `F6` 更换变量名、函数名等
+ `ctrl` + `k` 进入到高级模式
+ + `ctrl` + `u` 将选中的字符/行变成大写或小写

#### 查看
+ `ctrl` + `q` 查看注释，不但可以看到自己的注释，还可以看到PHP函数的注释
+ `ctrl` + `r` 查看本文件的函数结构
+ `ctrl` + `shift` + `F12` 打开资源管理器
+ `alt` + `←→` 切换代码标签页
+ `ctrl` + `shift` + `c` 复制绝对路径
+ `ctrl` + `shift` + `alt` + `c`复制相对路径
+ `shift` + `F1` 查看光标选中的php函数的文档，直接跳转到php.net

#### 光标移动
+ `ctrl` + `d` 向后选择一样的单词，常用于批量修改变量
+ `ctrl` + `B` 或 `鼠标中键` 或  找到变量或函数的定义(鼠标党福利)
+ `alt` + `↑↓` 切换函数
+ `F2` 查看下一个出错的地方

#### 搜索
+ `ctrl` + `p` 按照文件名搜索(巨好用)
+ `ctrl` + `f` 文本搜索
+ `ctrl` + `n` 按照类名进行搜索
+ `ctrl` + `g` 跳转到指定的行数
+ `ctrl` + `h` 替换文本
+ `ctrl` + `shift` + `f` 全局搜索文本
+ `双击shift` 搜索文件、文本等内容
+ `ctrl` + `e` 最近打开的文件
+ 

#### 其他
+ `ctrl` + `shift` + `t` 打开/关闭Terminal

#### git操作
+ `ctrl` + `k`
+ + `ctrl` + `c` git commit
+ + `ctrl` + `p` git push
+ + `ctrl` + `b` git checkout <branch>
+ + `ctrl` + `f` git fetch
+ + `ctrl` + `r` git rebase <branch>

## 断点调试
phpstorm结合xdebug来进行断点调试超级方便，以下介绍phpstorm调试大法的操作

#### 快捷键
+ `shift`+ `F10` 以release模式运行，无法进行debug
+ `alt`+ `F10` 以release模式运行，无法进行debug
+ `shift`+ `F9` 以debug模式运行
+ `alt`+ `F5` 以debug模式运行
+ `F7` 进入函数
+ `F8` 下一行
+ `shift` + `F8` 跳出函数
+ `F9` 继续运行
+ `ctrl` + `shift` + `F8` View Breakpoints
+ 

#### 一些方法

在watches窗口可以将你希望看到的变量过滤并展示出来，并且可以写表达式将复杂变量展示

`alt` + `F9` 可以光标指到哪里断点断在哪里，实现指哪断哪的功能

> 如果在一个for循环中，我希望在第100次断住，怎么操作？

如果在一处打断点，然后一直用鼠标一直点击运行，这样效率很低。更好的方法是点击`View Breakpoints`然后再`condition`中填入条件即可，例如`$i==100` 

## 功能

> Database Tool 数据库操作神器

感觉是可以媲美`Navicat`的操作数据库软件了，应该是`JetBrains`公司的`DataGrip`软件的缩小版，功能完全够用。尤其是`Run Script`的功能不会像`Navicat`的一样中途中断。`sql`语句的自动补全功能也比`navicat`的功能好用。

+ `F5` 在选中的时候或不选中的时候运行`sql`语句

> HTTP Client

差不多是PhpStorm里面内置的PostMan了，支持轻量的http访问。但是感觉功能还是差了挺多的，还不能模拟服务端，也没有import url的功能，暂时不建议使用。

> Analyse Xdebug Profile

根据`XDebug`插件产生的`profile`性能分析日志，对代码进行性能分析。

 

## 插件

> CodeGlance 

跟sublime text 一样的minimap

> Translation 翻译

+ `ctrl` + `shift` + `o` 打开翻译界面
+ `ctrl` + `shift` + `y` 翻译所选字符串

## 参考资料
[PhpStorm Tips](https://phpstorm.tips/)

[PhpStorm的几款必要插件](https://www.cnblogs.com/mclaoliu/archive/2018/05/04/8992522.html)
