# README.md 与 SUMMARY编写

使用语法
在Gitbook中所有文字的编写都使用Markdown语法。

README.md
这个文件相对于是一本Gitbook的简介，比如我们这本书的README.md :

# Gitbook 使用入门


> GitBook 是一个基于 Node.js 的命令行工具，可使用 Github/Git 和 Markdown 来制作精美的电子书。

本书将简单介绍如何安装、编写、生成、发布一本在线图书。
SUMMARY.md
这个文件相对于是一本书的目录结构。比如我们这本书的SUMMARY.md :

* [介绍](README.md)
* [基本安装](installation/README.md)
   * [Node.js安装](installation/nodejs-install.md)
   * [Gitbook安装](installation/gitbook-install.md)
   * [Gitbook命令行速览](installation/gitbook-cli.md)
* [图书项目结构](book/README.md)
   * [README.md 与 SUMMARY编写](book/file.md)
   * [目录初始化](book/prjinit.md)
* [图书输出](output/README.md)
   * [输出为静态网站](output/static.md)
   * [输出PDF](output/pdfandebook.md)
* [发布](publish/README.md)
   * [发布到Github Pages](publish/gitpages.md)
   * [发布到公司文档服务器](publish/companyserver.md)
* [结束](end/README.md)
SUMMARY.md基本上是列表加链接的语法。链接中可以使用目录，也可以使用。

# 图书项目结构

是Gitbook项目必备的两个文件，也就是一本最简单的gitbook也必须含有这两个文件，它们在一本Gitbook中具有不同的用处。

## 目录结构
Gitbook 使用简单的目录结构

```markdown
.
├── book.json
├── README.md
├── SUMMARY.md
├── chapter-1/
|   ├── README.md
|   └── something.md
└── chapter-2/
    ├── README.md
    └── something.md
简单的介绍下每个文件的作用

File	作用描述
book.json	记录电子书的配置 (可选)
README.md	前言 或者 电子书的介绍 必须
SUMMARY.md	电子书的目录 可选，参考Pages
GLOSSARY.md	术语表 ，可选，参考 Glossary
多语言
当使用多语言时，为每一种语言建立一个子目录，然后需要额外根目录建立一个文件 LANGS.md

# Languages

* [English](en/)
* [French](fr/)
* [Español](es/)
```