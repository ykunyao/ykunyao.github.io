---
title: Slides-cli
date: 2026-05-02 20:31:44
categories:
  - 项目记录
tags:
  - CLI
  - 工具
---

# slides-cli 🎬

终端 Markdown/HTML 幻灯片播放器。

用 Markdown 写 PPT，在终端里放，按 `e` 直接调 VS Code 改源文件，保存即刷新。

[repo](https://github.com/ykunyao/slides_cli)

## 安装

```bash
cd slides-cli
uv tool install .
uv tool update-shell   # 把 slides 命令加到 PATH
```

装完后在任何目录都能直接用 `slides`。

## 使用

```bash
slides show talk.md          # 播放 Markdown 幻灯片
slides show index.html       # 也支持 HTML（自动转 Markdown）
```

## 快捷键

| 键                | 功能                                     |
| ----------------- | ---------------------------------------- |
| ← → / j k / space | 翻页                                     |
| e                 | 编辑源文件（调 VS Code，保存后自动刷新） |
| r                 | 重新加载文件                             |
| g                 | 跳转到指定页                             |
| q                 | 退出                                     |

## 分页规则

Markdown 文件：

1. 优先按 `---`（水平线）切页
2. 没有 `---` 则按 `## `（二级标题）切页
3. 都没有就把整个文件当一页

HTML 文件：

1. 按 `<hr>` 切页
2. HTML 标签自动转为 Markdown 再渲染

## 视觉设计

纯白背景（`#fcfcfc`），全屏无边框，内容居中留白。代码块使用亮色模式高亮，语法着色清晰可见。

## 技术栈

- **Textual** — TUI 框架（键盘交互、布局、模态框）
- **Rich** — Markdown 渲染（标题、表格、代码高亮）
- **html2text** — HTML → Markdown 转换
- **uv** — Python 包管理
