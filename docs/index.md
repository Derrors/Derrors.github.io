# 基于mkdocs-material搭建个人静态博客(含支持的markdown语法)

## **本文主题**

---

1. mkdocs-material入门，包括安装、运行、发布至github-pages及个人站点

2. markdown语法，包括传统语法和mkdocs-material支持的扩展语法

## **mkdocs-material是什么**

---

符合google material ui规范的静态文档网站生成器，使用markdown进行文档书写

**mkdocs**

- python编写的markdown解释器、编译器，带有本地cli工具

- 自带基于Tornado的小型http服务，用于本地调试

- 内置一键式发布至GitHub Pages

- 内置mkdocs风格、readthedocs风格的主题，并支持自定义主题

- 支持调用python模块实现语法及渲染的扩展

**mkdocs-material**

- python模块，符合google material ui规范的mkdocs自定义主题

- 针对特定语法、功能做了渲染优化

- 根据客户端浏览器页面尺寸自动缩放，对PC、移动设备都友好

- 丰富的页面配色，多达19种主体配色和16种悬停链接文字配色

最佳实践: 建议仅使用[mkdocs-material](http://squidfunk.github.io/mkdocs-material/)官网支持的语法、功能，这样不会有渲染方面的异常，除非自己对mkdocs、mkdocs-material、html、js、css有一定的了解。

本文所有阐述的语法均是mkdocs-material官网推荐的。

## **写在前面**

---

1. 本文大部分内容均是个人理解，不保证准确性。

2. 本文主要是阐述markdown语法，因此关于mkdocs-material的高级配置、python markdown和pymdowx模块所支持的markdown语法不在本文阐述范围。有兴趣的可以自己到相应官网了解，具体如下:

	- [mkdocs](http://www.mkdocs.org)

	- [mkdocs-material](http://squidfunk.github.io/mkdocs-material/)

	- [python markdown](http://pythonhosted.org/Markdown/ "Markdown")

	- [pymdownx](http://facelessuser.github.io/pymdown-extensions/ "pymdown-extensions")
