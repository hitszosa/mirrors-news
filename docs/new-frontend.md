---
title: 镜像站新前端上线了
date: 2023-10-02
description: 了解新镜像站前端的开发历程和亮点。
tags: 
    - 公告
---

# 镜像站新前端上线了

> Rewrite it in Vue!

## 背景

镜像站原本使用的前端，是在哈工大校本部同学的帮助下，基于校本部镜像站的[前端项目](https://github.com/hitlug/mirror-web)修改而成。由于这个项目使用了 React 开发，而且采用的编程范式和依赖较旧，因此维护成本比较高。在衡量了重构成本和重写成本，以及参考了其他学校的镜像站前端项目之后，我们决定用 Nuxt 框架从头开发自己的镜像站前端。

## 开发历程

### 总体布局和组件

采用了三段式布局，即导航栏、主页面和页脚。其中导航栏的毛玻璃效果启发自 [Apple 网站](https://apple.com)，页脚设计启发自 [GitHub 网站](https://github.com)。在经历无数的 CSS 作战后，最终打磨出了一个非常优雅而通用的 UI/UX 设计。

### 镜像列表和侧边栏

镜像列表和侧边栏的设计启发自[南科大镜像站](https://mirrors.sustech.edu.cn)。青出于蓝而胜于蓝，我们总结了南科大镜像站的 UI 缺陷，并在开发中用更好的设计去解决这些缺陷。例如，我们的总体布局更舒适、易于阅读和统一，图标与字体大小比例正确，没有错误的标题层级，将「LiveCD & Software」栏目放在更显眼的位置等。

### 「获取 LiveCD 和软件」浮窗

该浮窗的设计同样启发自[南科大镜像站](https://mirrors.sustech.edu.cn)。由于组件库中没有能完全满足需求的现成组件，因此，我们结合网站总体的设计风格，开发了侧边选择滑块组件。美中不足的是，由于潜在的复杂交互逻辑，我们没有开发出像南科大镜像站那样的「标签页视图」。

### Markdown 文章渲染

采用了 GitHub 的样式，并在此基础上结合我们的设计风格修改而成。

### 新闻功能

新闻列表参考了 [GitHub 博客](https://github.blog)的设计。目前，新闻功能还在活跃开发阶段。~~事实上这篇文章只是为了演示一下新闻功能而已。~~

## 我要贡献

欢迎向我们的 GitHub 仓库提交 PR 或 Issue：<https://github.com/hitszosa/mirrors-frontend>。

