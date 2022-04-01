# 命令行

**还未翻译完成.....**

### 启动项参数

- `-A` 或 `--smarthome`
> 智能Home键，当光标在空白字符时，按下Home键会跳到实际字符前，`|||||char`(|代空格)，这时按下Home键，会跳到char前面，而不是最前面的空格


- `-B` 或 `--backup`
> 保存文件后会生成一个以波浪号为结尾的备份文件，同Vim的`set backup`


- `-C 目录路径` 或 `--backupdir=目录路径`
> `-B`的升级版，每次保存文件都会在指定目录产生一个备份文件，并以唯一的数字命名


- `-D` 或 `--boldtext`
> 对于界面，使用粗体来代替反显，它会覆盖`.nanorc`中的颜色配置


- `-E` 或 `--tabstospaces`
> 把Tab都变成空格，Tab教徒改信空格教 (确信)


- `-F` 或 `--multibuffer`
> 默认情况下，把文件读入新的缓冲区 (我没太看懂，如果有大佬知道这是啥可以反馈给我)


- `-G` 或 `--locking`
> 允许Vim式的文件锁 (我也不知道这是啥)


- `-H` 或 `--historylog`
> 保存最近100次的查找、替换和执行命令的记录，可以在之后的编辑中更好的复用


- `-I` 或 `--igonrercfiles`
> 忽略配置文件`.nanorc`


- `-J 列数` 或 `--guidestripe 列数`
> 在给定的列数会画上一条线，以便确定一行的字数


- `-K` 或 `--rawsequences`
> 这个直接放原文了，我不会翻译
> 
> Interpret escape sequences directly, instead of asking ncurses to translate them. (If you need this option to get some keys to work properly, it means that the terminfo terminal description that is used does not fully match the actual behavior of your terminal. This can happen when you ssh into a BSD machine, for example.) Using this option disables nano’s mouse support. 


- `-L` 或 `--nonewlines`
> 如果文件不以空行结尾，就自动添加空行，不过这可能会导致文件不可移植 (Non-POSIX)


- `-M` 或 `--trimblanks`
> 取消自动换行和自动对齐


- `-N` 或 `--noconvert`
> 禁止DOS和Mac格式的文件自动转换


- `-O` 或 `--bookstyle`
> 当自动对齐时，将任何空行视为段落的开头，除非开启自动缩进


- `-P` 或 `--positionlog`
> 对于最近200个打开过的文件，记录其最后的光标位置，再次打开它们时，光标会放到上次退出的位置


- `-Q "正则"` 或 `--quotestr="正则"`
> Set the regular expression for matching the quoting part of a line. The default value is "^([ \t]*([!#%:;>|}]|//))+". (Note that \t stands for a literal Tab character.) This makes it possible to rejustify blocks of quoted text when composing email, and to rewrap blocks of line comments when writing source code. 


- `-R` 或 `--restricted`
> Restricted mode: don’t read or write to any file not specified on the command line. This means: don’t read or write history files; don’t allow suspending; don’t allow spell checking; don’t allow a file to be appended to, prepended to, or saved under a different name if it already has one; and don’t make backup files. Restricted mode can also be activated by invoking nano with any name beginning with r (e.g. rnano).


- `-S` 或 `--softwrap`
> Display over multiple screen rows lines that exceed the screen’s width. (You can make this soft-wrapping occur at whitespace instead of rudely at the screen’s edge, by using also --atblanks.) (The old short option, -$, is deprecated.)


- `-T 数字` 或 `--tabsize=数字`
> Set the displayed tab length to number columns. The value of number must be greater than 0. The default value is 8.


- `-U` 或 `--quickblank`
> Make status-bar messages disappear after 1 keystroke instead of after 20. Note that option -c (--constantshow) overrides this. When option --minibar or --zero is in effect, --quickblank makes a message disappear after 0.8 seconds instead of after the default 1.5 seconds.


- `-V` 或 `--version`
> 显示Nano版本，但是不进入Nano


- `-W` 或 `--wordbounds`
> Detect word boundaries differently by treating punctuation characters as parts of words.


- `-X "字符"` 或 `--wordchars="字符"`
> Specify which other characters (besides the normal alphanumeric ones) should be considered as parts of words. When using this option, you probably want to omit -W (--wordbounds).


- `-Y name` 或 `--syntax=name`
> Specify the syntax to be used for highlighting. See Syntax Highlighting for more info.


- `-Z` 或 `--zap`
> Let an unmodified Backspace or Delete erase the marked region (instead of a single character, and without affecting the cutbuffer).


- `-a` 或 `--atblanks`
> When doing soft line wrapping, wrap lines at whitespace instead of always at the edge of the screen.


- `-b` 或 `--breaklonglines`
> Automatically hard-wrap the current line when it becomes overlong. (This option is the opposite of -w (--nowrap) — the last one given takes effect.)


- `-c` 或 `--constantshow`
> Constantly display the cursor position (line number, column number, and character number) on the status bar. Note that this overrides option -U (--quickblank).


- `-d` 或 `--rebinddelete`
> Interpret the Delete and Backspace keys differently so that both work properly. You should only use this option when on your system either Backspace acts like Delete or Delete acts like Backspace.


- `-e` 或 `--emptyline`
> Do not use the line below the title bar, leaving it entirely blank.


- `-f file` 或 `--rcfile=file`
> Read only this file for setting nano’s options, instead of reading both the system-wide and the user’s nanorc files.


- `-g` 或 `--showcursor`
> Make the cursor visible in the file browser (putting it on the highlighted item) and in the help viewer. Useful for braille users and people with poor vision.


- `-h` 或 `--help`
> Show a summary of command-line options and exit.


- `-i` 或 `--autoindent`
> Automatically indent a newly created line to the same number of tabs and/or spaces as the previous line (or as the next line if the previous line is the beginning of a paragraph).


- `-j` 或 `--jumpyscrolling`
> 滚动屏幕时，到最底下一行时，再向下移，则会用屏幕中间的那行替代第一行


- `-k` 或 `--cutfromcursor`
> Make the ’Cut Text’ command (normally ^K) cut from the current cursor position to the end of the line, instead of cutting the entire line.


- `-l` 或 `--linenumbers`
> 在文本左侧显示行数 (会和文本有一条边界)


- `-m` 或 `--mouse`
> 如果系统有权使用鼠标的话，开启鼠标支持。当开启鼠标支持时，按左键可以让光标移动到指定位置，双击同一位置可以开启选中模式，还可以点击底部提示栏。如果是有GUI的系统且鼠标服务正在运行，鼠标将会显示在窗口之上。文本仍然可以通过按住Shift键进行拖选。


- `-n` 或 `--noread`
> Treat any name given on the command line as a new file. This allows nano to write to named pipes: it will start with a blank buffer, and will write to the pipe when the user saves the "file". This way nano can be used as an editor in combination with for instance gpg without having to write sensitive data to disk first.


- `-o 目录` 或 `--operatingdir=目录`
> 设置操作目录，类似于`chroot`命令，保存文件时会保存在指定目录中


- `-p` 或 `--preserve`
> Preserve the ^Q (XON) and ^S (XOFF) sequences so data being sent to the editor can be stopped and started.


- `-q` 或 `--indicator`
> Display a "scrollbar" on the righthand side of the edit window. It shows the position of the viewport in the buffer and how much of the buffer is covered by the viewport.


- `-r number` 或 `--fill=number`
> Set the target width for justifying and automatic hard-wrapping at this number of columns. If the value is 0 or less, wrapping will occur at the width of the screen minus number columns, allowing the wrap point to vary along with the width of the screen if the screen is resized. The default value is -8.


- `-s "program [argument …]"` 或 `--speller="program [argument …]"`
> Use the given program to do spell checking and correcting. By default, nano uses the command specified in the SPELL environment variable. If SPELL is not set, and --speller is not specified either, then nano uses its own interactive spell corrector, which requires either hunspell or GNU spell to be installed.


- `-t` 或 `--saveonexit`
> Save a changed buffer without prompting (when exiting with ^X). This can be handy when nano is used as the composer of an email program. (The old form of the long option, --tempfile, is deprecated.)


- `-u` 或 `--unix`
> Save a file by default in Unix format. This overrides nano’s default behavior of saving a file in the format that it had. (This option has no effect when you also use --noconvert.)


- `-v` 或 `--view`
> Don’t allow the contents of the file to be altered: read-only mode. This mode allows the user to open also other files for viewing, unless --restricted is given too. (Note that this option should NOT be used in place of correct file permissions to implement a read-only file.)


- `-w` 或 `--nowrap`
> Do not automatically hard-wrap the current line when it becomes overlong. This is the default. (This option is the opposite of -b (--breaklonglines) — the last one given takes effect.)


- `-x` 或 `--nohelp`
> Expert mode: don’t show the two help lines at the bottom of the screen. This affects the location of the status bar as well, as in Expert mode it is located at the very bottom of the editor.
> 
> Note: When accessing the help system, Expert mode is temporarily disabled to display the help-system navigation keys.


- `-y` 或 `--afterends`
> 让`Ctrl+→` 和 `Ctrl+Del` 停在单词结尾而非单词开头


- `-z` 或 `--suspendable`
> Obsolete option; ignored. Suspension is enabled by default, reachable via ^T^Z. (If you want a plain ^Z to suspend nano, add bind ^Z suspend main to your nanorc.)


- `-%` 或 `--stateflags`
> Use the top-right corner of the screen for showing some state flags: I when auto-indenting, M when the mark is on, L when hard-wrapping (breaking long lines), R when recording a macro, and S when soft-wrapping. When the buffer is modified, a star (*) is shown after the filename in the center of the title bar.


- `-_` 或 `--minibar`
> Suppress the title bar and instead show information about the current buffer at the bottom of the screen, in the space for the status bar. In this "minibar" the filename is shown on the left, followed by an asterisk if the buffer has been modified. On the right are displayed the current line and column number, the code of the character under the cursor (in Unicode format: U+xxxx), the same flags as are shown by --stateflags, and a percentage that expresses how far the cursor is into the file (linewise). When a file is loaded or saved, and also when switching between buffers, the number of lines in the buffer is displayed after the filename. This number is cleared upon the next keystroke, or replaced with an [i/n] counter when multiple buffers are open. The line plus column numbers and the character code are displayed only when --constantshow is used, and can be toggled on and off with M-C. The state flags are displayed only when --stateflags is used.


- `-0` 或 `--zero`
> Hide all elements of the interface (title bar, status bar, and help lines) and use all rows of the terminal for showing the contents of the buffer. The status bar appears only when there is a significant message, and disappears after 1.5 seconds or upon the next keystroke. With M-Z the title bar plus status bar can be toggled. With M-X the help lines.


- `-!` 或 `--magic`
> When neither the file’s name nor its first line give a clue, try using libmagic to determine the applicable syntax.


***

**此篇翻译贡献者: Lemonix、Sherlock**