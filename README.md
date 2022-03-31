# Nano Tutorial


## 介绍
Nano编辑器简易教程

人生苦短，我用Nano

Nano是一个简单且友好的编辑器，相比于Vim的复杂和Emacs的庞大，Nano显得如此友善


## 教程

#### 移动
- `CTRL-b` 向左移动，同 **\<Left\>**
- `CTRL-f` 向右移动，同 **\<Right\>**
- `CTRL-p` 向上移动，同 **\<Up\>**
- `CTRL-n` 向下移动，同 **\<Down\>**
- `CTRL-a` 移动到行首，同 **\<Home\>**
- `CTRL-e` 移动到行末，同 **\<End\>**
- `CTRL-v` 下翻页，同 **\<PageDown\>**
- `CTRL-y` 上翻页，同 **\<PageUp\>**
- `CTRL-Left` 向左跳一个单词
- `CTRL-Right` 向右跳一个单词

#### 跳转与匹配
- ALT-\ 跳到文件开头
- ALT-/ 跳到文件末尾
- ALT-g 跳到指定行号
- ALT-] 跳到匹配的括号或者Tag
- CTRL-w 查找字符串
- ALT-w 重复上次查找
- CTRL-\ 查找替换
- ALT-r 查找替换，同 CTRL-\
- ALT-( 跳转到上一个段落
- ALT-) 跳转到下一个段落

#### 文本操作
- ALT-a ALT-} 选择一个块并缩进
- ALT-a ALT-{ 选择一个块并反缩进
- CTRL-d 删除光标下字符
- CTRL-h 删除光标左边字符
- CTRL-j 调整段落


#### 文件操作
- CTRL-o <Enter> 保存文件 
- CTRL-r ALT-f 在 Nano 中打开新文件
- CTRL-r CTRL-t 使用文件管理器寻找并打开文件
- ALT-< 切换到前一个文件，同 ALT-, 
- ALT-> 切换到后一个文件，同 ALT-.
- CTRL-q 退出 Nano

#### 选择
- CTRL-k 剪贴从光标处到行末的文本
- ALT-a ALT-^ 复制高亮的选中文本到剪贴板
- ALT-a ALT-k 剪贴高亮的选中文本到剪贴板
- ALT-^ 复制当前行到剪贴板
- CTRL-u 粘贴剪贴板里的文本到光标处
- ALT-a 开始选择文本用于复制或者剪贴，再次按 ALT-a 会取消选择
- CTRL-^ 开始选择文本用于复制或者剪贴，同 ALT-a，CTRL 和 6一起按下
- Shift-方向键 同上

#### 操作管理
- ALT-u 撤销
- ALT-e 重复

#### 自定义
- `ALT-x` 是否允许显示底部帮助信息
- `ALT-c` 是否显示光标位置
- `ALT-o` 是否允许多行编辑
- `ALT-s` 是否允许平滑卷屏
- `ALT-$` 是否允许自动换行
- `ALT-p` 是否显示空格和制表符
- `ALT-y` 是否允许语法高亮
- `ALT-h` 是否允许智能 Home 键
- `ALT-i` 是否允许自动缩进
- `ALT-k` 是否允许剪贴到行末
- `ALT-l` 是否允许硬性自动换行
- `ALT-q` 是否允许展开制表符为空格
- `ALT-b` 是否允许备份文件
- `ALT-f` 是否允许加载文件到新的缓存
- `ALT-m` 是否允许鼠标
- `ALT-#` 是否显示行号
- `CTRL-g` 显示帮助

## 编写者
Lemonix **整理自官方文档和知乎**