

# 常用设置

- 加到排除列表，可见但默认不会被搜到：
  - WebStorm 认为 `node_modules` 是「library root」，并将其标记为「Excluded」，这样的好处是 **不会污染全文搜索**，但构建产物没有这样的福利，需要手动设置
  - 右键菜单 **Mark Directory as** → **Excluded**
  - 或者 **Settings** → **Directories** → **Exclude files**
- 高亮有变更的目录
  - **Settings** → **Version Control** → **Confirmation**，勾选「Highlight directories that contain modified files in the Project tree」



# 插件

- `Atom Material Icons` - 文件图标插件
- `Rainbow Bracket` - 彩虹括号
- `Code Glance Pro` - 代码缩略图
- `String Manipulation` - 字符串右键切换大小写
- `Tabnine` - AI代码提示
- `Draw.io` - 流程图插件



# 高频快捷键

## 快速编辑

| 快捷键 | 预设值 | 功能                     | 设置路径                                                     | 说明                                           |
| ------ | ------ | ------------------------ | ------------------------------------------------------------ | ---------------------------------------------- |
| ⇧⇥     | ⇧⇥     | 取消缩进（反向 Tab）     | **Main Menu** → **Edit** → **Edit Code Actions** → **Unindent Line or Selection** | 无法理解居然有人不知道...                      |
| ⌘D     | ⌘D     | 删除光标所在行（所选行） | **Editor Actions** → **Delete Line**                         | 很多在线编辑器，如 ACE、CodeMirror 等也都是 ⌘D |
| ⌥↑     | ⌥↑     | 光标所在处的语句上移一行 | **Main Menu** → **Code** → **Move Statement Up**             | 注意是语句，比单纯的移动行更智能               |
| ⌥↓     | ⌥↓     | 光标所在处的语句下移一行 | **Main Menu** → **Code** → **Move Statement Down**           | 同上                                           |
| ⌘/     | ⌘/     | 单行注释                 | **Main Menu** → **Code** → **Comment Actions** → **Comment with Line Comment** |                                                |
| 🌈 ⇧⌘/  | ⌃⇧/    | 多行注释                 | **Main Menu** → **Code** → **Comment Actions** → **Comment with Block Comment** | 需要改系统快捷键，对应系统快捷键是呼出帮助     |
| ⇧⌘F    | ⇧⌘F    | 格式化代码               | **Main Menu** → **Code** → **Code Formatting Actions** → **Format Code** | 不要养成习惯                                   |
| 🌈 ⇧⌘J  | ⌃⇧J    | 合并所选行               | **Editor Actions** → **Join Lines**                          |                                                |
| ⇧⌘X    | ⇧⌘X    | 切换大小写               | **Editor Actions** → **Toggle Case**                         |                                                |
| ⌥⌘↓    | ⌥⌘↓    | 向下复制一行             | **Editor Actions** → **Duplicate Entire Lines**              | 我找不到向上复制行的命令了 😭                   |
| ⌘⌫     | ⌘⌫     | 从光标处删除到整个词首   | **Editor Actions** → **Delete to Word Start**                |                                                |
| ⌘⌦     | ⌘⌦     | 从光标处删除到整个词尾   | **Editor Actions** → **Delete to Word End**                  |                                                |
| ⌥⌫     | ⌥⌫     | 从光标处删除到分词的词首 | **Editor Actions** → **Delete to Word Start in Different "CamelHumps" Mode** |                                                |
| ⌥⌦     | ⌥⌦     | 从光标处删除到分词的词尾 | **Editor Actions** → **Delete to Word End in Different "CamelHumps" Mode** |                                                |

## 移动光标

| 快捷键 | 预设值 | 功能                   | 设置路径                                              | 说明                               |
| ------ | ------ | ---------------------- | ----------------------------------------------------- | ---------------------------------- |
| ⌘←     | ⌘←     | 移动光标至行首         | **Editor Actions** → **Move Caret to Line Start**     | 忽略行首空白                       |
| ⌘→     | ⌘→     | 移动光标至行尾         | **Editor Actions** → **Move Caret to Line End**       | 忽略行尾空白                       |
| 🌈 ⌘↑   | ⌘↖     | 移动光标至文首         | **Editor Actions** → **Move Caret to Text Start**     |                                    |
| 🌈 ⌘↓   | ⌘↘     | 移动光标至文尾         | **Editor Actions** → **Move Caret to Text End**       |                                    |
| ⌥←     | ⌥←     | 移动光标到上一个词     | **Editor Actions** → **Move Caret to Previous Word**  | 功能描述不是很全面，最好自己试一下 |
| ⌥→     | ⌥→     | 移动光标到下一个词     | **Editor Actions** → **Move Caret to Next Word**      | 功能描述不是很全面，最好自己试一下 |
| ⇧⌘\    | ⇧⌘\    | 移动光标到对应的括号处 | **Editor Actions** → **Move Caret to Matching Brace** | 吸收自 VSCode                      |

## 选择文本

> 💡 ⇧ 的「圈选」Buff。

| 快捷键 | 预设值 | 功能                               | 设置路径                                                     | 说明 |
| ------ | ------ | ---------------------------------- | ------------------------------------------------------------ | ---- |
| 🌈 ⇧⌘↑  | ⇧⌘↖    | 移动光标至文首，选中经过的文本     | **Editor Actions** → **Move Caret to Text Start with Selection** |      |
| 🌈 ⇧⌘↓  | ⇧⌘↘    | 移动光标至文末，选中经过的文本     | **Editor Actions** → **Move Caret to Text End with Selection** |      |
| ⇧⌘←    | ⇧⌘←    | 移动光标至行首，选中经过的文本     | **Editor Actions** → **Move Caret to Line Start with Selection** |      |
| ⇧⌘→    | ⇧⌘→    | 移动光标至行尾，选中经过的文本     | **Editor Actions** → **Move Caret to Line End with Selection** |      |
| ⌥⇧←    | ⌥⇧←    | 移动光标到上一个词，选中经过的文本 | **Editor Actions** → **Move Caret to Previous Word with Selection** |      |
| ⌥⇧→    | ⌥⇧→    | 移动光标到下一个词，选中经过的文本 | **Editor Actions** → **Move Caret to Next Word with Selection** |      |

## 快速导航

| 快捷键   | 预设值      | 功能             | 设置路径                                                     | 说明            |
| -------- | ----------- | ---------------- | ------------------------------------------------------------ | --------------- |
| ⇧⌘R      | ⇧⌘R         | 根据名字查找文件 | **Main Menu** → **Navigate** → **Goto by Name Actions** → **Go to File...** | R 表示 Resource |
| ⇧⌘T      | ⇧⌘T         | 根据名字查找类   | **Main Menu** → **Navigate** → **Goto by Name Actions** → **Go to Class...** | T 表示 Type     |
| 🌈 ⌘Click | F3 / ⌃Click | 跳到定义或使用处 | **Main Menu** → **Navigate** → **Goto by Reference Actions** → **Go to Declaration or Usages** |                 |

## 查找替换

| 快捷键 | 预设值 | 功能                                 | 设置路径                                                     | 说明 |
| ------ | ------ | ------------------------------------ | ------------------------------------------------------------ | ---- |
| 🌈 ⌘F   | -      | 当前文件内搜索                       | **Main Menu** → **Edit** → **Find** → **Find...**            |      |
| 🌈 ⌘R   | -      | 当前文件内替换                       | **Main Menu** → **Edit** → **Find** → **Replace...**         |      |
| ⌘G     | ⌘G     | 查找并将光标移动到下一个搜索命中文本 | **Main Menu** → **Edit** → **Find** → **Find Next / Move to Next Occurrence** |      |
| ⇧⌘G    | ⇧⌘G    | 查找并将光标移动到上一个搜索命中文本 | **Main Menu** → **Edit** → **Find** → **Find Previous / Move to Previous Occurrence** |      |
| ⌃H     | ⌃H     | 全局内容搜索                         | **Main Menu** → **Edit** → **Find** → **Find in Files...**   |      |
| 🌈 ⌃⇧H  | -      | 全局内容替换                         | **Main Menu** → **Edit** → **Find** → **Replace in Files...** |      |
| 🌈 ⌥⌘G  | ⇧⌘G    | 查找引用（文件、Symbol）             | **Main Menu** → **Edit** → **Find Usages** → **Find Usages** |      |

## 多点编辑

> Sublime 创新了多点编辑以来，几乎所有的 IDE、编辑器，甚至 Web 端的 [Ace](https://link.juejin.cn?target=https%3A%2F%2Face.c9.io)、[CodeMirror](https://link.juejin.cn?target=https%3A%2F%2Fcodemirror.net) 等都在一夜之间都实现了该功能。

在创建多个光标后，结合箭头、移动光标快捷键等，绝对是炫技提效必备。

| 快捷键     | 预设值     | 功能                               | 设置路径                                                     | 说明                                                   |
| ---------- | ---------- | ---------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------ |
| ⌥Click     | ⌥Click     | 增加光标                           | **Editor Actions** → **Add or Remove Caret**                 | 基础                                                   |
| ⌃⌘G        | ⌃⌘G        | 选中所有选中的文本，或光标所在的词 | **Main Menu** → **Edit** → **Find** → **Select All Occurrences** | 选择后，每个词的光标位置一致                           |
| 🌈 ⇧⌘L      | ⌥⌘G        | 所有选中行末添加光标               | **Main Menu** → **Edit** → **Editor Select Actions** → **Add Carets to Ends of Selected Lines** |                                                        |
| 🌈 ⌥⇧↑      | -          | 向上复制光标                       | **Editor Actions** → **Clone Caret Above**                   |                                                        |
| 🌈 ⌥⇧↓      | -          | 向下复制光标                       | **Editor Actions** → **Clone Caret Below**                   |                                                        |
| ⌥⇧鼠标拖拽 | ⌥⇧鼠标拖拽 | 纵向拖出一条光标                   | -                                                            | 类似连续多次向上或向下复制光标的效果，但附加带选中效果 |

## 通用

| 快捷键 | 预设值 | 功能                               | 设置路径                                                     | 说明             |
| ------ | ------ | ---------------------------------- | ------------------------------------------------------------ | ---------------- |
| ⌘1     | ⌘1     | 展示快速修复菜单                   | **Other** → **Show Quick-Fixes**                             | 有病没病都可以按 |
| 🌈 ⌃`   | ⌥F12   | 展示 / 隐藏 Terminal               | **Tool Windows** → **Terminal**                              | VSCode 习惯      |
| 🌈 ⌘\   | -      | 编辑器向右切屏                     | **Main Menu** → **Window** → **Editor Tabs** → **Split Right** |                  |
| 🌈 ⌥⌘\  | -      | 编辑器向下切屏                     | **Main Menu** → **Window** → **Editor Tabs** → **Split Down** |                  |
| 🌈 F2   | ⇧F6    | 重命名（文件，变量名、类名等符号） | **Main Menu** → **Refactor** → **Rename...**                 |                  |
| 🌈 ⌥Z   | -      | 开启 / 关闭代码软折行              | **Main Menu** → **View** → **Active Editor** → **Soft Wrap** | 习自 VSCode      |

## Git

| 快捷键 | 预设值 | 功能                            | 设置路径                                                 | 说明                                                    |
| ------ | ------ | ------------------------------- | -------------------------------------------------------- | ------------------------------------------------------- |
| 🌈 ⌘K   | -      | Git Commit                      | **Version Control System** → **Commit...**               | 同时把 Terminal Clear 的快捷键也改成 ⌘K，和系统保持一致 |
| ⌃V     | ⌃V     | VCS 操作弹层                    | **Version Control System** → **VCS Operations Popup...** | 这样很多操作就不需要去文件树上右键了                    |
| 🌈 ⌥⇧⌘B | -      | 显示/隐藏编辑器左侧的 Git Blame | **Version Control System** → **Annotate**                | 看到臭代码想 **B**lame 谁的时候，常用                   |

## 特有功能

| 快捷键 | 预设值 | 功能               | 设置路径                                                     | 说明                                    |
| ------ | ------ | ------------------ | ------------------------------------------------------------ | --------------------------------------- |
| ⌘D     | ⌘D     | 文件比较           | **Main Menu** → **Views** → **Actions on Pairs of Files** → **Compare Files** | 在文件树上的 ⌘D，触发文件比较，非常有用 |
| ⇧⌘N    | ⇧⌘N    | 新建草稿文件       | **Main Menu** → **File** → **File Open Actions** → **New** → **Scratch File** | -                                       |
| 🌈 ⌃⌘P  | -      | 切换演示模式       | **View** → **Appearance** → **Toggle Presentation mode**     | 给小伙伴讲解代码的时候用                |
| ⌥⌘U    | ⌥⌘U    | 弹窗展示依赖关系图 | **Plugins** → **Diagrams** → **Show Diagram Popups**         |                                         |
| ⌥⇧⌘U   | ⌥⇧⌘U   | 弹窗展示依赖关系图 | **Plugins** → **Diagrams** → **Show Diagram**                |                                         |





> https://juejin.cn/post/7271184462934147135





