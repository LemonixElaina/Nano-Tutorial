# Nano Tutorial


***


# 介绍

#### Nano 编辑器简易教程
**人生苦短，我用Nano**，Nano是一个简单且友好的编辑器，相比于Vim的复杂和Emacs的庞大，Nano可太简单了，如此的易学，绝对适合你！

[Nano官网](https://www.nano-editor.org/)

截止2022/3/31 (YYYY/MM/DD)，目前还没有翻译完，仍然有很多官方文档的英文原文，以后会慢慢翻译的，想要协助翻译的可以提交Issue

这个文档翻译起来工程量很大，如果您愿意，可以选择用捐赠的方式支持我一下，我把支付渠道放到了此文件结尾

***


# 教程
- `nano 文件名` 使用Nano编辑文件
**编辑器中^为 Ctrl 键，M为 Meta 键，即键盘上的 Alt 键**

## 快捷键
#### 移动光标
- `Ctrl-b` 向左移动，同 **\<Left>**
- `Ctrl-f` 向右移动，同 **\<Right>**
- `Ctrl-p` 向上移动，同 **\<Up>**
- `Ctrl-n` 向下移动，同 **\<Down>**
- `Ctrl-a` 移动到行首，同 **\<Home>**
- `Ctrl-e` 移动到行末，同 **\<End>**
- `Ctrl-v` 下翻页，同 **\<PageDown>**
- `Ctrl-y` 上翻页，同 **\<PageUp>**
- `Ctrl-Left` 向左跳一个单词
- `Ctrl-Right` 向右跳一个单词

#### 跳转与匹配
- `Alt-\` 跳到文件开头
- `Alt-/` 跳到文件末尾
- `Alt-g` 跳到指定行号
- `Alt-]` 跳到匹配的括号或者Tag
- `Alt-w` 重复上次查找
- `Alt-r` 查找替换，同 `Ctrl-\`
- `Alt-(` 跳转到上一个段落
- `Alt-)` 跳转到下一个段落
- `Ctrl-w` 查找字符串

#### 文本操作
- `Alt-a Alt-}` 选择一个块并缩进
- `Alt-a Alt-{` 选择一个块并反缩进
- `Ctrl-d` 删除光标下字符
- `Ctrl-h` 删除光标左边字符
- `Ctrl-j` 调整段落

#### 文件操作
- `Alt-<` 切换到前一个文件，同 `Alt-,`
- `Alt->` 切换到后一个文件，同 `Alt-.`
- `Ctrl-o <Enter>` 保存文件 
- `Ctrl-r Alt-f` 在 Nano 中打开新文件
- `Ctrl-r Ctrl-t` 使用文件管理器寻找并打开文件

#### 选择与粘贴
- `Alt-^` 复制当前行到剪贴板
- `Alt-a Alt-^` 复制高亮的选中文本到剪贴板
- `Alt-a Alt-k` 剪贴高亮的选中文本到剪贴板
- `Alt-a` 开始选择文本用于复制或者剪贴，再次按 `Alt-a` 会取消选择
- `Ctrl-u` 粘贴剪贴板里的文本到光标处
- `Ctrl-k` 剪贴从光标处到行末的文本
- `Ctrl-^` 开始选择文本用于复制或者剪贴，同 `Ctrl-6`、`Alt-a`或`Shift-方向键`

#### 操作管理
- `Alt-u` 撤销
- `Alt-e` 重复
- `Alt-:` 开始或停止录制宏
- `Alt-;` 运行最近录制的宏

#### 自定义
- `Alt-x` 是否允许显示底部帮助信息
- `Alt-c` 是否显示光标位置
- `Alt-o` 是否允许多行编辑
- `Alt-s` 是否允许平滑卷屏
- `Alt-$` 是否允许自动换行
- `Alt-p` 是否显示空格和制表符
- `Alt-y` 是否允许语法高亮
- `Alt-h` 是否允许智能 Home 键
- `Alt-i` 是否允许自动缩进
- `Alt-k` 是否允许剪贴到行末
- `Alt-l` 是否允许硬性自动换行
- `Alt-q` 是否允许展开制表符为空格
- `Alt-b` 是否允许备份文件
- `Alt-f` 是否允许加载文件到新的缓存
- `Alt-m` 是否允许鼠标
- `Alt-#` 是否显示行号
- `Ctrl-g` 显示帮助


## 配置文件 `.nanorc`
**见[RcFile.md](RcFile.md)**


## 命令行
#### 安装Nano
- **Ubuntu** & **Debian** : `apt install nano`
- **Arch** & **Manjaro** : `pacman -S nano`
- **Fedora** : `dnf install nano`

#### 命令行参数
**见[Options.md](Options.md)**


***


# 编写者
***Lemonix*** **整理自官方文档和知乎**

![捐赠](Donate.jpg)
_这不是我的名字，我未成年，只能用我爸的身份证_