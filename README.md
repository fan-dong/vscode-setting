# vscode 配置

## 插件
```
1、Auto Close Tag
2、Auto Complete Tag
3、Auto Import
4、Auto Rename Tag
5、Babel ES6/ES7
6.koroFileHeader
7.Vue 2 Snippets
8、Chinese (Simplified) Language Pack for Visual Studio Code
9、Code Spell Checker
10、Color Highlight
11、Guides
12、Import Cost
13、Indenticator
14、JavaScript (ES6) code snippets
15、Live Server
16、Manta's Stylus Supremacy
17、markdownlint
18、vscode-icons
19、open in browser
20、Path Autocomplete
21、Path Intellisense
22、Vetur
23、Element UI Snippets
24、翻译
25、language-stylus
26、stylus
27、Highlight Matching Tag
28、Material Theme Kit
29、Project Manager
30、NPM-Scripts


```
## 配置json

```

  {
  "editor.renderIndentGuides": false,
  "editor.fontSize": 16,
  "editor.quickSuggestionsDelay": 0,
  "files.trimTrailingWhitespace": true,
  "breadcrumbs.enabled": true,
  "editor.wordWrap": "on",
    // vscode默认启用了根据文件类型自动设置tabsize的选项
  "editor.detectIndentation": false,
  // 重新设定tabsize
  "editor.tabSize": 2,
  // #每次保存的时候自动格式化
  "editor.formatOnSave": false,
  // #每次保存的时候将代码按eslint格式进行修复
  "eslint.autoFixOnSave": true,
  // 添加 vue 支持
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    {
      "language": "vue",
      "autoFix": true
    }
  ],
  //  #让prettier使用eslint的代码格式进行校验
  "prettier.eslintIntegration": true,
  //  #去掉代码结尾的分号
  "prettier.semi": true,
  //  #使用带引号替代双引号
  "prettier.singleQuote": true,
  //  #让函数(名)和后面的括号之间加个空格
  "javascript.format.insertSpaceBeforeFunctionParenthesis": false,
  // #这个按用户自身习惯选择
  "vetur.format.defaultFormatter.html": "js-beautify-html",
  // #让vue中的js按编辑器自带的ts格式进行格式化
  "vetur.format.defaultFormatter.js": "vscode-typescript",
  "vetur.format.defaultFormatterOptions": {
    "js-beautify-html": {
      "wrap_line_length": 20000,
      "wrap_attributes": "auto",
      "end_with_newline": false
      // #vue组件中html代码格式化样式
    }
  },
  // 格式化stylus, 需安装Manta's Stylus Supremacy插件
  "stylusSupremacy.insertColons": false, // 是否插入冒号
  "stylusSupremacy.insertSemicolons": false, // 是否插入分好
  "stylusSupremacy.insertBraces": false, // 是否插入大括号
  "stylusSupremacy.insertNewLineAroundImports": false, // import之后是否换行
  "stylusSupremacy.insertNewLineAroundBlocks": false,
  "[javascript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "liveServer.settings.donotShowInfoMsg": true, // 两个选择器中是否换行
  // 头部注释
  "fileheader.customMade": {
    "Author": "Fred",
    "Date": "Do not edit",
    "LastEditors": "Fred",
    "LastEditTime": "Do not edit",
    "Description": "file content"
  },
  "fileheader.cursorMode": {},
  "files.autoSave": "onFocusChange",
  "editor.fontWeight": "500",
  "workbench.sideBar.location": "right",
  "vsicons.dontShowNewVersionMessage": true,
  "atomKeymap.promptV3Features": true,
  "workbench.colorTheme": "Material",
  "workbench.iconTheme": "vscode-icons"
}


```
## 新建vue代码片段

>文件-->首选项-->用户代码片段-->点击新建代码片段--取名vue.json 确定。
>删除不要的代码,入自己写的.vue模板。
```
{
  "Print to console": {
      "prefix": "vue",
      "body": [
          "<template>",
          "  <div></div>",
          "</template>",
          "",
          "<script>",
          "import {",
          "  mapState,",
          "  mapGetters,",
          "  mapMutations,",
          "  mapActions,",
          "} from 'vuex';",
          "",
          "export default {",
          "  name: '',",
          "  components: {},",
          "  filters: {},",
          "  directives: {},",
          "  data() {",
          "    return {",
          "      ",
          "    };",
          "  },",
          "  watch: {",
          "      ",
          "  },",
          "  computed: {",
          "    ...mapState({",
          "      // ...",
          "    }),",
          "    ...mapGetters([",
          "      // ...",
          "    ]),",
          "  },",
          "  methods: {",
          "    ...mapMutations([",
          "      // ...",
          "    ]),",
          "    ...mapActions([",
          "      // ...",
          "    ]),",
          "  },",
          "  created() {",
          "    ",
          "  },",
          "  mounted() {",
          "    ",
          "  },",
          "}",
          "</script>",
          "",
          "<style lang='scss' scoped>",
          "$4",
          "</style>"
      ],
      "description": "Log output to console"
  }
}


```
## vscode常用快捷键总结
>记住快捷键能够提高工作效率
```

Ctrl+Shift+P,F1 展示全局命令面板

Ctrl+P 快速打开最近打开的文件

Ctrl+Shift+N 打开新的编辑器窗口

Ctrl+Shift+W 关闭编辑器

Ctrl + X 剪切

Ctrl + C 复制

Alt + up/down 移动行上下

Shift + Alt up/down 在当前行上下复制当前行

Ctrl + Shift + K 删除行

Ctrl + Enter 在当前行下插入新的一行

Ctrl + Shift + Enter 在当前行上插入新的一行

Ctrl + Shift + | 匹配花括号的闭合处，跳转

Ctrl + ] 或 [ 行缩进

Home 光标跳转到行头

End 光标跳转到行尾

Ctrl + Home 跳转到页头

Ctrl + End 跳转到页尾

Ctrl + up/down 行视图上下偏移

Alt + PgUp/PgDown 屏视图上下偏移

Ctrl + Shift + [ 折叠区域代码

Ctrl + Shift + ] 展开区域代码

Ctrl + / 添加关闭行注释

Shift + Alt +A 块区域注释

Alt + Z 添加关闭词汇包含

导航快捷键

Ctrl + T 列出所有符号

Ctrl + G 跳转行

Ctrl + P 跳转文件

Ctrl + Shift + O 跳转到符号处

Ctrl + Shift + M 或 Ctrl + J 打开问题展示面板

F8 跳转到下一个错误或者警告

Shift + F8 跳转到上一个错误或者警告

Ctrl + Shift + Tab 切换到最近打开的文件

Alt + left / right 向后、向前

Ctrl + M 进入用Tab来移动焦点

Ctrl + F 查询

Ctrl + H 替换

F3 / Shift + F3 查询下一个/上一个

Alt + Enter 选中所有出现在查询中的

Ctrl + D 匹配当前选中的词汇或者行，再次选中-可操作

多行光标快捷键

Alt + Click 插入光标-支持多个

Ctrl + Alt + up/down 上下插入光标-支持多个

Ctrl + U 撤销最后一次光标操作

Shift + Alt + I 插入光标到选中范围内所有行结束符

Ctrl + I 选中当前行

Ctrl + Shift + L 选择所有出现在当前选中的行-操作

Ctrl + F2 选择所有出现在当前选中的词汇-操作

Shift + Alt + right 从光标处扩展选中全行

Shift + Alt + left 收缩选择区域

Shift + Alt + (drag mouse) 鼠标拖动区域，同时在多个行结束符插入光标

Ctrl + Shift + Alt + (Arrow Key) 也是插入多行光标的[方向键控制]

Ctrl + Shift + Alt + PgUp/PgDown 也是插入多行光标的[整屏生效]

Esc Esc 连续按两次Esc键取消多行光标

Shift + Alt + F 格式化代码

F12 跳转到定义处

Alt + F12 代码片段显示定义

Ctrl + K F12 在其他窗口打开定义处

Ctrl + . 快速修复部分可以修复的语法错误

Shift + F12 显示所有引用

F2 重命名符号

Ctrl + Shift + . / , 替换下个值

编辑器管理快捷键

Ctrl + F4, Ctrl + W 关闭编辑器

Ctrl + |切割编辑窗口

Ctrl + 1/2/3 切换焦点在不同的切割窗口

Ctrl + Shift + PgUp/PgDown 切换标签页的位置

文件管理快捷键

Ctrl + N 新建文件

Ctrl + O 打开文件

Ctrl + S 保存文件

Ctrl + Shift + S 另存为

Ctrl + F4 关闭当前编辑窗口

Ctrl + W 关闭所有编辑窗口

Ctrl + Shift + T 撤销最近关闭的一个文件编辑窗口

Ctrl + Enter 保持开启

Ctrl + Shift + Tab 调出最近打开的文件列表，重复按会切换

Ctrl + Tab 与上面一致，顺序不一致

Ctrl + P 复制当前打开文件的存放路径

Ctrl + R 打开当前编辑文件存放位置【文件管理器】

显示快捷键

F11 切换全屏模式

Ctrl + =/- 放大 / 缩小

Ctrl + B 侧边栏显示隐藏

Ctrl + Shift + E 资源视图和编辑视图的焦点切换

Ctrl + Shift + F 打开全局搜索

Ctrl + Shift + G 打开Git可视管理

Ctrl + Shift + D 打开DeBug面板

Ctrl + Shift + X 打开插件市场面板

Ctrl + Shift + H 在当前文件替换查询替换

Ctrl + Shift + J 开启详细查询

Ctrl + Shift + V 预览Markdown文件【编译后】

Ctrl + K v 在边栏打开渲染后的视图【新建】

调试快捷键

F9 添加解除断点

F5 启动调试、继续

F11 / Shift + F11 单步进入 / 单步跳出

F10 单步跳过

集成终端快捷键

Ctrl + ` 打开集成终端

Ctrl + Shift + ` 创建一个新的终端

Ctrl + C 复制所选

Ctrl + V 复制到当前激活的终端

Shift + PgUp / PgDown 页面上下翻屏

Ctrl + Home / End 滚动到页面头部或尾部

```
