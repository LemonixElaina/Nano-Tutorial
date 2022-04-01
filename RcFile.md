# 配置文件

**还未翻译完成.....**

### 目前支持的设置有:

- `set afterends`
> 使 `Ctrl+Right` 和 `Ctrl+Delete` 停在单词结尾而非单词开头


- `set allow_insecure_backup`
> When backing up files, allow the backup to succeed even if its permissions can’t be (re)set due to special OS considerations. You should NOT enable this option unless you are sure you need it.


- `set atblanks`
> When soft line wrapping is enabled, make it wrap lines at blank characters (tabs and spaces) instead of always at the edge of the screen.


- `set autoindent`
> Automatically indent a newly created line to the same number of tabs and/or spaces as the previous line (or as the next line if the previous line is the beginning of a paragraph).


- `set backup`
> When saving a file, back up the previous version of it, using the current filename suffixed with a tilde (~).


- `set backupdir "directory"`
> Make and keep not just one backup file, but make and keep a uniquely numbered one every time a file is saved — when backups are enabled with set backup or --backup or -B. The uniquely numbered files are stored in the specified directory.


- `set boldtext`
> Use bold instead of reverse video for the title bar, status bar, key combos, function tags, line numbers, and selected text. This is overridden by setting the options titlecolor, statuscolor, keycolor, functioncolor, numbercolor, and/or selectedcolor.


- `set bookstyle`
> When justifying, treat any line that starts with whitespace as the beginning of a paragraph (unless auto-indenting is on).


- `set brackets "characters"`
> Set the characters treated as closing brackets when justifying paragraphs. This may not include blank characters. Only closing punctuation (see set punct), optionally followed by the specified closing brackets, can end sentences. The default value is ""')>]}".


- `set breaklonglines`
> Automatically hard-wrap the current line when it becomes overlong.


- `set casesensitive`
> Do case-sensitive searches by default.


- `set constantshow`
> Constantly display the cursor position on the status bar. Note that this overrides quickblank.


- `set cutfromcursor`
> Use cut-from-cursor-to-end-of-line by default, instead of cutting the whole line.


- `set emptyline`
> Do not use the line below the title bar, leaving it entirely blank.


- `set errorcolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the status bar when an error message is displayed. The default value is bold,white,red. See set keycolor for valid color names.


- `set fill number`
> Set the target width for justifying and automatic hard-wrapping at this number of columns. If the value is 0 or less, wrapping will occur at the width of the screen minus number columns, allowing the wrap point to vary along with the width of the screen if the screen is resized. The default value is -8.


- `set functioncolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the concise function descriptions in the two help lines at the bottom of the screen. See set keycolor for valid color names.


- `set guidestripe number`
> Draw a vertical stripe at the given column, to help judge the width of the text. (The color of the stripe can be changed with set stripecolor.)


- `set historylog`
> Save the last hundred search strings and replacement strings and executed commands, so they can be easily reused in later sessions.


- `set indicator`
> Display a "scrollbar" on the righthand side of the edit window. It shows the position of the viewport in the buffer and how much of the buffer is covered by the viewport.


- `set jumpyscrolling`
> Scroll the buffer contents per half-screen instead of per line.


- `set keycolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the shortcut key combos in the two help lines at the bottom of the screen. Valid names for the foreground and background colors are: red, green, blue, magenta, yellow, cyan, white, and black. Each of these eight names may be prefixed with the word light to get a brighter version of that color. The word grey or gray may be used as a synonym for lightblack.
> 
> On terminal emulators that can do at least 256 colors, other valid (but unprefixable) color names are: pink, purple, mauve, lagoon, mint, lime, peach, orange, latte, rosy, beet, plum, sea, sky, slate, teal, sage, brown, ocher, sand, tawny, brick, crimson, and normal — where normal means the default foreground or background color. On such emulators, the color may also be specified as a three-digit hexadecimal number prefixed with #, with the digits representing the amounts of red, green, and blue, respectively. This tells nano to select from the available palette the color that approximates the given values.
> 
> Either fgcolor or ,bgcolor may be left out, and the pair may be preceded by bold and/or italic (separated by commas) to get a bold and/or slanting typeface, if your terminal can do those.


- `set linenumbers`
> Display line numbers to the left of the text area. (Any line with an anchor additionally gets a mark in the margin.)


- `set locking`
> Enable vim-style lock-files for when editing files.


- `set magic`
> When neither the file’s name nor its first line give a clue, try using libmagic to determine the applicable syntax. (Calling libmagic can be relatively time consuming. It is therefore not done by default.)


- `set matchbrackets "characters"`
> Specify the opening and closing brackets that can be found by bracket searches. This may not include blank characters. The opening set must come before the closing set, and the two sets must be in the same order. The default value is "(<[{)>]}".


- `set minibar`
> Suppress the title bar and instead show information about the current buffer at the bottom of the screen, in the space for the status bar. In this "minibar" the filename is shown on the left, followed by an asterisk if the buffer has been modified. On the right are displayed the current line and column number, the code of the character under the cursor (in Unicode format: U+xxxx), the same flags as are shown by set stateflags, and a percentage that expresses how far the cursor is into the file (linewise). When a file is loaded or saved, and also when switching between buffers, the number of lines in the buffer is displayed after the filename. This number is cleared upon the next keystroke, or replaced with an [i/n] counter when multiple buffers are open. The line plus column numbers and the character code are displayed only when set constantshow is used, and can be toggled on and off with M-C. The state flags are displayed only when set stateflags is used.


- `set minicolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the minibar. (When this option is not specified, the colors of the title bar are used.) See set keycolor for valid color names.


- `set mouse`
> Enable mouse support, so that mouse clicks can be used to place the cursor, set the mark (with a double click), or execute shortcuts.


- `set multibuffer`
> When reading in a file with ^R, insert it into a new buffer by default.


- `set noconvert`
> Don’t convert files from DOS/Mac format.


- `set nohelp`
> Don’t display the help lists at the bottom of the screen.


- `set nonewlines`
> Don’t automatically add a newline when a text does not end with one. (This can cause you to save non-POSIX text files.)


- `set nowrap`
> Deprecated option since it has become the default setting. When needed, use unset breaklonglines instead.


- `set numbercolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for line numbers. See set keycolor for valid color names.


- `set operatingdir "directory"`
> Nano will only read and write files inside "directory" and its subdirectories. Also, the current directory is changed to here, so files are inserted from this directory. By default, the operating directory feature is turned off.


- `set positionlog`
> Save the cursor position of files between editing sessions. The cursor position is remembered for the 200 most-recently edited files.


- `set preserve`
> Preserve the XON and XOFF keys (^Q and ^S).


- `set promptcolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the prompt bar. (When this option is not specified, the colors of the title bar are used.) See set keycolor for valid color names.


- `set punct "characters"`
> Set the characters treated as closing punctuation when justifying paragraphs. This may not include blank characters. Only the specified closing punctuation, optionally followed by closing brackets (see set brackets), can end sentences. The default value is "!.?".


- `set quickblank`
> Make status-bar messages disappear after 1 keystroke instead of after 20. Note that option constantshow overrides this. When option minibar or zero is in effect, quickblank makes a message disappear after 0.8 seconds instead of after the default 1.5 seconds.


- `set quotestr "regex"`
> Set the regular expression for matching the quoting part of a line. The default value is "^([ \t]*([!#%:;>|}]|//))+". (Note that \t stands for a literal Tab character.) This makes it possible to rejustify blocks of quoted text when composing email, and to rewrap blocks of line comments when writing source code.


- `set rawsequences`
> Interpret escape sequences directly, instead of asking ncurses to translate them. (If you need this option to get some keys to work properly, it means that the terminfo terminal description that is used does not fully match the actual behavior of your terminal. This can happen when you ssh into a BSD machine, for example.) Using this option disables nano’s mouse support.


- `set rebinddelete`
> Interpret the Delete and Backspace keys differently so that both work properly. You should only use this option when on your system either Backspace acts like Delete or Delete acts like Backspace.


- `set regexp`
> Do regular-expression searches by default. Regular expressions in nano are of the extended type (ERE).


- `set saveonexit`
> Save a changed buffer automatically on exit (^X); don’t prompt. (The old form of this option, set tempfile, is deprecated.)


- `set scrollercolor fgcolor,bgcolor`
> Use this color combination for the indicator alias "scrollbar". (On terminal emulators that link to a libvte older than version 0.55, using a background color here does not work correctly.) See set keycolor for valid color names.


- `set selectedcolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for selected text. See set keycolor for valid color names.


- `set showcursor`
> Put the cursor on the highlighted item in the file browser, and show the cursor in the help viewer, to aid braille users and people with poor vision.


- `set smarthome`
> Make the Home key smarter. When Home is pressed anywhere but at the very beginning of non-whitespace characters on a line, the cursor will jump to that beginning (either forwards or backwards). If the cursor is already at that position, it will jump to the true beginning of the line.


- `set softwrap`
> Display lines that exceed the screen’s width over multiple screen lines. (You can make this soft-wrapping occur at whitespace instead of rudely at the screen’s edge, by using also set atblanks.)


- `set speller "program [argument …]"`
> Use the given program to do spell checking and correcting. See --speller for details.


- `set spotlightcolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for highlighting a search match. The default value is black,lightyellow. See set keycolor for valid color names.


- `set stateflags`
> Use the top-right corner of the screen for showing some state flags: I when auto-indenting, M when the mark is on, L when hard-wrapping (breaking long lines), R when recording a macro, and S when soft-wrapping. When the buffer is modified, a star (*) is shown after the filename in the center of the title bar.


- `set statuscolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the status bar. See set keycolor for valid color names.


- `set stripecolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the vertical guiding stripe. See set keycolor for valid color names.


- `set suspendable`
> Obsolete option; ignored. Suspension is enabled by default, reachable via ^T^Z. (If you want a plain ^Z to suspend nano, add bind ^Z suspend main to your nanorc.)


- `set tabsize number`
> Use a tab size of number columns. The value of number must be greater than 0. The default value is 8.


- `set tabstospaces`
> Convert each typed tab to spaces — to the number of spaces that a tab at that position would take up.


- `set titlecolor [bold,][italic,]fgcolor,bgcolor`
> Use this color combination for the title bar. See set keycolor for valid color names.


- `set trimblanks`
> Remove trailing whitespace from wrapped lines when automatic hard-wrapping occurs or when text is justified.


- `set unix`
> Save a file by default in Unix format. This overrides nano’s default behavior of saving a file in the format that it had. (This option has no effect when you also use set noconvert.)


- `set whitespace "characters"`
> Set the two characters used to indicate the presence of tabs and spaces. They must be single-column characters. The default pair for a UTF-8 locale is "»·", and for other locales ">.".


- `set wordbounds`
> Detect word boundaries differently by treating punctuation characters as part of a word.


- `set wordchars "characters"`
> Specify which other charactrs (besides the normal alphanumeric ones) should be considered as parts of words. When using this option, you probably want to unset wordbounds.


> et zap`
> Let an unmodified Backspace or Delete erase the marked region (instead of a single character, and without affecting the cutbuffer).


- `set zero`
> de all elements of the interface (title bar, status bar, and help lines) and use all rows of the terminal for showing the contents of the buffer. The status bar appears only when there is a significant message, and disappears after 1.5 seconds or upon the next keystroke. With M-Z the title bar plus status bar can be toggled. With M-X th> 


***


**此篇翻译贡献者: Lemonix**
