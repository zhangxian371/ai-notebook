# AI Notebook

一个轻量、零依赖的个人学习笔记站，用静态 HTML 整理技术知识、阅读思考和专题资料。

项目以 `index.html` 作为资料入口，每篇笔记都是可以独立打开的 HTML 页面，适合直接在本地阅读，也可以部署到 GitHub Pages。当前内容横跨前端基础、Linux、GitHub Pages、游戏设计、哲学和音乐文本解读。

## 在线访问

- GitHub Pages：<https://zhangxian371.github.io/ai-notebook/>
- GitHub 仓库：<https://github.com/zhangxian371/ai-notebook>

## 现有内容

- **前端基础**：HTML、HTTP、REST、CSS 历史及交互式示例
- **Linux 学习**：程序、进程、信号与 `/proc` 文件系统
- **项目实践**：联机飞行棋架构学习报告、贪吃蛇游戏设计方案
- **后端科普**：面向 C++ 初学者的 Node.js、HTTP 与 WebSocket 讲解
- **GitHub Pages**：静态网页托管指南与完整实践攻略
- **哲学思考**：王阳明“格物”“诚意”与《传习录》解读
- **文本解读**：《无用清净梦》《一如年少模样》等歌词赏析

## 项目特点

- 无构建流程、无第三方依赖，浏览器即可运行
- 首页按“项目与工程、编程与系统、阅读与思考”分类展示笔记
- 笔记页面支持独立设计，也提供 `style/notes.css` 公共样式和多套主题色
- 适合直接托管在 GitHub Pages 等静态网站服务上

## 本地运行

最简单的方式是直接打开 `index.html`。

也可以在项目目录启动一个本地静态服务器：

```bash
python3 -m http.server 8000
```

然后访问：

```text
http://localhost:8000
```

## 目录结构

```text
ai-notebook/
├── index.html                         # 笔记导航首页
├── style/
│   └── notes.css                     # 笔记页面公共样式与主题
├── html是什么.html                    # HTML 入门科普
├── html笔记.html                      # HTML 与 HTTP 学习笔记
├── html资源与REST.html                # Resource、REST 与缓存
├── css历史.html                       # CSS 历史与交互示例
├── linux-process-notes.html           # Linux 程序与进程笔记
├── Node.js_给C++初学者的科普报告.html   # Node.js、HTTP 与 WebSocket 科普
├── 联机飞行棋_给C++初学者的学习报告.html # 联机游戏架构学习报告
├── GitHub Pages 托管指南.html          # GitHub Pages 快速指南
├── GitHub Pages 全攻略.html            # GitHub Pages 完整攻略
├── 贪吃蛇游戏核心设计方案.html          # 游戏设计文档
├── wang-yangming-gewu.html            # 王阳明格物与诚意解读
├── wang-yangming-chuanxi-lu-6.html    # 《传习录》第六条解读
└── *-歌词解读.html                    # 音乐文本解读
```

## 添加新笔记

1. 在仓库根目录新建 HTML 文件。
2. 如需复用统一样式，引入公共样式表，并在 `body` 上选择主题类：

   ```html
   <link rel="stylesheet" href="style/notes.css">
   <body class="theme-html">
   ```

3. 在 `index.html` 对应分类中新增一张卡片，填写相对链接、标题和简介。

首页只索引仓库中真实存在的页面。新增或删除笔记时，应同步维护首页卡片，避免产生失效链接。

## 部署到 GitHub Pages

仓库是纯静态网站，可以直接使用 GitHub Pages：

1. 进入仓库的 **Settings → Pages**。
2. 选择从分支部署。
3. 选择 `master` 分支和根目录 `/`。
4. 保存并等待 GitHub 完成发布。

仓库地址：<https://github.com/zhangxian371/ai-notebook>
