# 常用设置

## 需手动设置

- 登录账号同步设置：可以同步主题、插件、自定义设置、快捷键映射等
  - 左下角 Account 菜单「Turn on Settings Sync...」
- 开启内嵌提示
  - 设置：关键词「inlayhint」，能勾选的都勾选，能选「all」的都选「all」

## 可复制下方推荐设置

- 启动记住全屏：上次退出程序的时候如果是全屏则再次启动的时候就是全屏
  - 设置：**Window: Restore Fullscreen**，勾选
- 文件树缩进设置：默认的文件树缩进层级太小，甚至无法辨别文件与目录的关系，看得眼疼。
  - 设置：**Workbench → Tree: Indent**，默认 8，改成 16 或 20
- 显示空白字符
  - 设置：**Editor: Render Whitespace**，选择「all」
- 取消中文标点高亮
  - 设置：**Editor → Unicode Highlight: Ambiguous Characters**，取消勾选
- 开启带颜色的缩进线：代替了 Rainbow Brackets 插件，此插件可以卸载了
  - 设置：**Editor → Guides: Bracket Pairs**，选择 true

## 推荐设置

```json
// settings.json
{
  "files.autoSave": "afterDelay", // 自动保存
  // 文件自动延迟保存
  "files.autoSaveDelay": 5000,
  "files.autoGuessEncoding": true,
  // 控制列表和树是否具有平滑滚动效果。
  "workbench.list.smoothScrolling": true,
  // 控制是否启用平滑插入动画
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.find.addExtraSpaceOnTop": false,
  "editor.smoothScrolling": true,
  "editor.cursorBlinking": "smooth",
  "editor.mouseWheelZoom": true,
  "editor.formatOnPaste": true,
  "editor.formatOnType": true,
  "editor.formatOnSave": true,
  "editor.wordWrap": "on",
  "editor.guides.bracketPairs": true,
  //"editor.bracketPairColorization.enabled": true, (此设置vscode在较新版本已默认开启)
  "editor.suggest.snippetsPreventQuickSuggestions": false,
  "editor.acceptSuggestionOnEnter": "smart",
  "editor.suggestSelection": "recentlyUsed",
  "window.dialogStyle": "custom",
  "debug.showBreakpointsInOverviewRuler": true,
  "workbench.tree.indent": 16, // 文件树缩进
  "window.restoreFullscreen": true, // 上次退出程序的时候如果是全屏则再次启动的时候就是全屏
  "editor.renderWhitespace": "all", // 显示空白字符
  "editor.unicodeHighlight.ambiguousCharacters": false, // 取消中文标点高亮
  "editor.guides.bracketPairs": true, // 开启带颜色的缩进线
}
```

# 插件

## 必备插件

- `ESLint` - 代码检查工具
- `prettier` - 【代码格式化工具】支持超多语言，一键格式化，美化代码格式
- `EditorConfig for VS Code` 配置同步插件
- `Stylelint` - CSS的代码检查工具
- `Auto rename Tag` - 同步修改标签
- `Auto Close Tag` - 自动补全结束标签
  - 新版Vscode原生已支持，但不支持不支持在  `.vue` 文件中的自动闭合，暂时建议安装

- `HTML CSS Support`
- `TypeScript Vue Plugin (Volar)`
- `Vue Language Features (Volar)`
- `Vue 3 Snippets` 代码片段提示
- `ES7+ React/Redux/React-Native snippets`
- `Typescript React code snippets`

## 推荐插件

- `GitLens` - git管理工具
- `Markdown Preview Enhanced`
- `Comment Translate`- 源码阅读辅助
- `Tailwind CSS IntelliSense` 
- `WindiCSS IntelliSense`
- `Path Intellisense` - 【路径补全】在输入路径时，有智能提示补全
- `Doxygen Documentation Generator` - 【文档生成器】写注释和文档时非常好用
- `Todo Tree` - 团队协作注释高亮
- `css navigation` - 跳转到样式定义的位置
- `open in browser` - `alt + B` 打开浏览器打开html
- `Spelling checker for source code` 拼写检查插件
- `DotENV` 环境变量.env语法高亮
- `Live Server` - 本地启动代理服务器用于
- `Turbo Console Log` 快捷键ctrl + alt + L (Windows) or ctrl + option + L (Mac)快速生成log
- `Project Manager`- 多项目管理工具

## 美化插件

- `Material Icon Theme` - 美化文件图标
- `One Dark Pro` - 主题
- `Moonlight`- 主题
- `vscode-icons` 官方图标库
- `Chinese (Simplified) (简体中文)`
- `Error Lens` - 【错误提示】可以将原先显示的问题显示在对应行右侧并高亮
- `Image preview` - 【图像预览】可以预览引入的图像
- `CodeSnap` - 【代码截图】一款非常好用的代码截图插件
- `Heighlight Matching Tag` - 鼠标停留成对tag高亮
- `Color Highlight` 颜色高亮显示
- `indent-rainbow` 彩虹缩进
- `Svg Preview` svg图片预览
- `Better Comments` 注释扩展分类
- `Image preview` 侧边预览css图片

## 其它

- `CodeGeeX2` - AI生成代码

- `Code Runner` - 【代码运行工具】支持多种语言，语言运行环境需自己配置

  ```json
  // 推荐修改配置：
  {
    "code-runner.runInTerminal": true,
    "code-runner.saveAllFilesBeforeRun": true,
    "code-runner.saveFileBeforeRun": true
  }
  ```

- `Docker`

- `Remote - SSH` - 【ssh连接】连接远程服务器或虚拟机

- `Code Spell Checker` - 检查单词拼写错误

- `Paramter Hints` - 提示函数参数类型

- `Quokka.js` - 实时显示打印输出

- `CONSOLOG` - 可以自动生成log，并显示相关信息 `ctrl alt L`。

- `TypeScript Import Sorter` - 引入排序

- `Git History`

- `GitLens — Git supercharged`

- `Todo Tree` 显示TODO树

- `Doxygen Documentation Generator` 快速生成文档注释 [配置](https://blog.csdn.net/my_id_kt/article/details/122852676)

- `Version Lens` 依赖版本提示

- `Draw.io Integration` - 流程图插件



# 高频快捷键

唤出 VSCode 快捷键自定义界面：

- 快捷键（二级跳）：⌘K ⌘S
- 命令面板搜「keyboard」，找到「Preferences: Open Keyboard Shortcuts」

带 🌈 标记表示需要自定义。



##  快速编辑

| 快捷键 | 预设值 | 功能                     | Command                              | 说明                                                 |
| ------ | ------ | ------------------------ | ------------------------------------ | ---------------------------------------------------- |
| ⇧⇥     | ⇧⇥     | 取消缩进（反向 Tab）     | `outdent`                            |                                                      |
| 🌈 ⌘D   | ⌘⇧K    | 删除光标所在行（所选行） | `editor.action.deleteLines`          |                                                      |
| ⌥↑     | ⌥↑     | 所选行/光标所在行上移    | `editor.action.moveLinesUpAction`    | 没有 WebStorm 智能                                   |
| ⌥↓     | ⌥↓     | 所选行/光标所在行下移    | `editor.action.moveLinesDownAction`  | 没有 WebStorm 智能                                   |
| ⌘/     | ⌘/     | 单行注释                 | `editor.action.toggleLineComment`    |                                                      |
| 🌈 ⇧⌘/  | ⌥⇧A    | 多行注释                 | `editor.action.blockComment`         | 需要改系统快捷键，对应系统快捷键是呼出帮助           |
| ⌥⇧F    | ⌥⇧F    | 格式化代码               | `editor.action.formatDocument`       | 💥 和 WebStorm 不一样                                 |
| 🌈 ⇧⌘J  | ⌃J     | 合并所选行               | `editor.action.joinLines`            |                                                      |
| 🌈 ⇧⌘X  | -      | 切换成大写               | `editor.action.transformToUppercase` | 没有 WebStorm 好用，可以一个快捷键在大小写间来回切换 |
| 🌈 ⌥⇧⌘X | -      | 切换成小写               | `editor.action.transformToLowercase` | 前面的快捷键上附加一个 ⌥                             |
| 🌈 ⌥⌘↑  | ⌥⇧↑    | 向上复制一行             | `editor.action.copyLinesUpAction`    |                                                      |
| 🌈 ⌥⌘↓  | ⌥⇧↓    | 向上复制一行             | `editor.action.copyLinesDownAction`  |                                                      |
| 🌈 ⌘⌫   | ⌥⌫     | 从光标处删除到整个词首   | `deleteWordLeft`                     | VSCode ⌘⌫ 默认为到行首，先解除之                     |
| 🌈 ⌘⌦   | ⌥⌦     | 从光标处删除到整个词尾   | `deleteWordRight`                    |                                                      |
| 🌈 ⌥⌫   | ⌃⌥⌫    | 从光标处删除到分词的词首 | `deleteWordPartLeft`                 |                                                      |
| 🌈 ⌥⌦   | ⌃⌥⌦    | 从光标处删除到分词的词尾 | `deleteWordPartRight`                |                                                      |

## 移动光标

| 快捷键 | 预设值 | 功能                   | Command                         | 说明                 |
| ------ | ------ | ---------------------- | ------------------------------- | -------------------- |
| ⌘↑     | ⌘↑     | 移动光标至文首         | `editor.action.goToTopHover`    |                      |
| ⌘↓     | ⌘↓     | 移动光标至文尾         | `editor.action.goToBottomHover` |                      |
| ⌘←     | ⌘←     | 移动光标至行首         | `cursorHome`                    | 忽略行首空白         |
| ⌘→     | ⌘→     | 移动光标至行尾         | `cursorEnd`                     | 但是不会忽略行尾空白 |
| ⌥←     | ⌥←     | 移动光标到上一个词     | `cursorWordLeft`                |                      |
| ⌥→     | ⌥→     | 移动光标到下一个词     | `cursorWordRight`               |                      |
| ⌥⇧\    | ⌥⇧\    | 移动光标到对应的括号处 | `editor.action.jumpToBracket`   |                      |

## 选择文本

| 快捷键 | 预设值 | 功能                               | Command                 | 说明 |
| ------ | ------ | ---------------------------------- | ----------------------- | ---- |
| ⇧⌘↑    | ⇧⌘↑    | 移动光标至文首，选中经过的文本     | `cursorTopSelect`       |      |
| ⇧⌘↓    | ⇧⌘↓    | 移动光标至文末，选中经过的文本     | `cursorBottomSelect`    |      |
| ⇧⌘←    | ⇧⌘←    | 移动光标至行首，选中经过的文本     | `cursorHomeSelect`      |      |
| ⇧⌘→    | ⇧⌘→    | 移动光标至行尾，选中经过的文本     | `cursorEndSelect`       |      |
| ⌥⇧←    | ⌥⇧←    | 移动光标到上一个词，选中经过的文本 | `cursorWordLeftSelect`  |      |
| ⌥⇧→    | ⌥⇧→    | 移动光标到下一个词，选中经过的文本 | `cursorWordRightSelect` |      |

## 快速导航

| 快捷键 | 预设值 | 功能                     | Command                           | 说明                           |
| ------ | ------ | ------------------------ | --------------------------------- | ------------------------------ |
| ⌘P     | ⌘P     | 根据名字搜索文件等资源   | `workbench.action.quickOpen`      | 💥 和 WebStorm 设的不一样       |
| ⌘T     | ⌘T     | 命令面板查找 Symbol 模式 | `workbench.action.showAllSymbols` | 和 WebStorm 的查找类型有点类似 |
| ⌘Click | ⌘Click | 跳到定义                 | -                                 |                                |

## 查找替换

| 快捷键 | 预设值 | 功能                                 | Command                                 | 说明                     |
| ------ | ------ | ------------------------------------ | --------------------------------------- | ------------------------ |
| ⌘F     | ⌘F     | 文件内搜索                           | `actions.find`                          |                          |
| ⌥⌘F    | ⌥⌘F    | 文件内替换                           | `editor.action.startFindReplaceAction`  | 💥 和 WebStorm 设的不一样 |
| ⌘G     | ⌘G     | 查找并将光标移动到下一个搜索命中文本 | `editor.action.nextMatchFindAction`     |                          |
| ⇧⌘G    | ⇧⌘G    | 查找并将光标移动到上一个搜索命中文本 | `editor.action.previousMatchFindAction` |                          |
| 🌈 ⌃H   | ⇧⌘F    | 全局内容搜素                         | `workbench.action.findInFiles`          |                          |
| 🌈 ⌃⇧H  | ⇧⌘H    | 全局内容替换                         | `workbench.action.replaceInFiles`       |                          |
| 🌈 ⌥⌘G  | ⌥⇧F12  | 查找引用                             | `references-view.findReferences`        | 💥 不支持文件             |

## 多点编辑

在创建多个光标后，结合箭头、移动光标快捷键等，绝对是炫技提效必备。

| 快捷键     | 预设值     | 功能                               | Command                                             | 说明                                                    |
| ---------- | ---------- | ---------------------------------- | --------------------------------------------------- | ------------------------------------------------------- |
| ⌥Click     | ⌥Click     | 增加光标                           | 无                                                  | 基础                                                    |
| 🌈 ⌃⌘G      | ⌃⌘L        | 选中所有选中的文本，或光标所在的词 | `editor.action.selectHighlights`                    | 💥 和 WebStorm 不一样的是，VSCode 选中后所有的光标在词尾 |
| 🌈 ⇧⌘L      | ⌥⇧I        | 所有选中行末添加光标               | `editor.action.insertCursorAtEndOfEachLineSelected` |                                                         |
| 🌈 ⌥⇧↑      | ⌥⌘↑        | 向上复制光标                       | `editor.action.insertCursorAbove`                   |                                                         |
| 🌈 ⌥⇧↓      | ⌥⌘↓        | 向下复制光标                       | `editor.action.insertCursorBelow`                   |                                                         |
| ⌥⇧鼠标拖拽 | ⌥⇧鼠标拖拽 | 纵向拖出一条光标                   | -                                                   | 类似连续多次向上或向下复制光标的效果，但附加带选中效果  |

## 通用

| 快捷键      | 预设值             | 功能                                       | Command                            | 说明                                     |
| ----------- | ------------------ | ------------------------------------------ | ---------------------------------- | ---------------------------------------- |
| 🌈 ⌘1        | ⌘.                 | 展示快速修复菜单                           | `editor.action.quickFix`           | 有病没病都可以按                         |
| ⌃`     | ⌃` | 展示/隐藏 Terminal | `workbench.action.terminal.toggleTerminal` |                                    |                                          |
| ⌘\          | ⌘\                 | 编辑器向右切屏                             | `workbench.action.splitEditor`     |                                          |
| 🌈 ⌥⌘\       | ⌘K ⌘\              | 编辑器向下切屏                             | `workbench.action.splitEditorDown` |                                          |
| ⏎           | ⏎                  | 重命名文件                                 | `renameFile`                       | 💥 和 WebStorm 不一样，保持系统的原汁原味 |
| ⌥Z          | ⌥Z                 | 代码软折行                                 | `editor.action.toggleWordWrap`     |                                          |

## 特有功能

| 快捷键 | 预设值 | 功能               | Command                                    | 说明               |
| ------ | ------ | ------------------ | ------------------------------------------ | ------------------ |
| ⇧⌘P    | ⇧⌘P    | 展示命令面板       | `workbench.action.showCommands`            | Sublime 最大的创举 |
| ⌘K ⌘S  | ⌘K ⌘S  | 打开快捷键偏好设置 | `workbench.action.openGlobalKeybindings`   |                    |
| ⌘B     | ⌘B     | 显示 / 隐藏侧边栏  | `workbench.action.toggleSidebarVisibility` |                    |











> PS：
>
> - [入坑 VSCode，看这一篇就够了](https://juejin.cn/post/7273435446587211812)
> - [2023年最新最全 VSCode 插件推荐](https://juejin.cn/post/7205753233599578170)
> - [你的 vscode 配置真的舒服么？](https://juejin.cn/post/7165056807704985608)
> - [良心提醒：这些你常用的vscode 扩展，应该卸载啦](https://juejin.cn/post/7274879238652723260)(注意：虽然很多功能Vscode已提供支持，但可能对Vue或者React支持并不友好)



