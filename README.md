<p align="center">
	<a><img width="100px" src="https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/Logo.png"/></a>
</p>
<p align="center">
	<a href="https://github.com/flydoos/WinASAR/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/flydoos/WinASAR?style=flat-square"></a>
	<a href="https://www.microsoft.com/zh-cn/download/details.aspx?id=17718"><img src="https://img.shields.io/badge/platform-windows-lightgrey.svg?style=flat-square"/></a>
	<a href="https://github.com/flydoos/WinASAR/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/flydoos/WinASAR?style=flat-square"></a>
	<a href="https://github.com/flydoos/WinASAR/tags"><img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/flydoos/WinASAR?style=flat-square"></a>
	<a href="https://github.com/flydoos/WinASAR/releases"><img src="https://img.shields.io/github/downloads/flydoos/WinASAR/total.svg?style=flat-square"/></a>
</p>
<p align="center">
	<img src="https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/ClickStar.png"/>
</p>

# 👀WinASAR文件管理工具（最好用的ASAR文件压缩/解压工具）

WinASAR文件管理工具（也叫：WinASAR文件压缩/解压工具、WinASAR文件打包/解包工具）由“牛A与牛C之间”开发制作，这是一款高仿 WinRAR 制作的 Electron ASAR 文件管理工具，部分功能也参考了 7-Zip。本程序主要功能用于 .Asar 文件的压缩与解压，除此之外，还支持轻量级 Windows 资源管理器功能，**本程序适用于 Windows 下所有 Electron ASAR 文件**。

近期，在制作 [飞书消息防撤回补丁](https://github.com/flydoos/FeiShuRevokeMsgPatcher)，然后接触到了 .Asar 格式文件，上网一搜发现这种文件居然要安装 node.js 环境，然后通过 npm 命令行才能进行文件的打包与提取（也就是压缩和解压），找了一圈发现存在个别的 Asar 小工具，但功能都比较单一也不怎么好看，于是乎，自己分析ASAR文件协议，然后动手做一个高仿 WinRAR 的 WinASAR 文件管理工具，希望大家使用起来就跟WinRAR一样，毫无违和感。

## 🖥️主要功能

1. 支持单选或多选文件、文件夹压缩成 .Asar 格式文件

2. 支持把 .Asar 格式文件解压到指定目录

3. 支持往已存在的 .Asar 文件中追加其他文件、删除文件、以及重命名

4. 支持测试 .Asar 文件是否存在错误

5. 支持 WinASAR 内置文件查看器，用于查看大文件，且支持文本搜索以及文件编码切换

6. 支持轻量级 Windows 资源管理功能，可实现文件、文件夹的复制（可自动创建不重名副本）、删除操作支持放入系统回收站、支持重命名等

7. 支持文件夹 “..” 返回上一层目录

8. 支持 Windows 目录下查找文件，以及支持 .Asar 内部查找文件

9. 支持右键菜单新建文件、新建文件夹

10. 支持文件列表自定义查看方式，可选择列表查看、或详细资料查看

11. 支持文件列表自定义排序方式，可选择不同字段进行排序，支持正序、倒序

12. 支持友好展示文件大小，自动适配 Bytes、KB、MB、GB 等不同单位

13. 支持创建 .Asar 文件格式关联，关联后双击可直接使用 WinASAR 打开

14. 支持创建桌面快捷方式

15. 支持自动保存配置信息，包括：设置信息，查看方式，排序方式，列表各个字段宽度，窗口大小等

## 📰知识科普

**什么是 ASAR 文件？**

[ASAR 格式文件](https://github.com/electron/asar/) 是一种由 Electron 开发的专用于 Electron 应用程序的归档文件格式（ASAR 全称：Atom Shell Archive，现在 Atom Shell 已改名为 Electron）。它的工作方式类似于 .tar 归档文件，即将多个文件和文件夹整合成单个文件，但不同于 .tar.gz 或 .zip 等格式，.asar 文件在存储时不进行压缩，而是保持原始文件数据的连续性，从而实现高效的随机访问。

## 🔗下载地址

**下载地址：[⚡️最新版 WinASAR 文件管理工具 下载](https://github.com/flydoos/WinASAR/releases/latest)**

其他推荐：[🦇钉钉消息防撤回补丁](https://github.com/flydoos/DingTalkRevokeMsgPatcher) | [📖飞书消息防撤回补丁](https://github.com/flydoos/FeiShuRevokeMsgPatcher) | [🔖查看作者更多作品](https://github.com/flydoos)

## 📷截图

![Screenshot](https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/Screenshot-1.4.0.png)

![Screenshot](https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/Screenshot-List-1.0.0.png)

![Screenshot](https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/Screenshot-View-1.0.0.png)

## 🔨使用方法

1. 首先，你的系统需要满足以下条件：

    * Windows XP 或更高版本。
    * [.NET Framework 4.0](https://www.microsoft.com/zh-cn/download/details.aspx?id=17718) 或更高版本。**低于此版本在打开程序时可能无反应，或者直接报错**。

2. **以管理员身份运行本程序**

3. 个人作者开发的软件，**杀毒软件可能会弹出警告，请放行且添加程序目录到信任白名单。**

设置文件格式关联后的效果：

![Screenshot](https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/Association.png)

## ❓常见问题

1、为什么不支持系统右键菜单，直接进行压缩与解压？由于Windows各个版本的右键菜单存在较大差异，暂时没空逐个适配，其次，系统右键菜单太多，会影响用户体验，如果要求此功能的人较多，后续有空会考虑支持。

## ❤联系我

QQ群：223541319 （催更请进群）

博客：https://www.cnblogs.com/flydoos

官网：https://www.wuleba.com （我的软件博客，大家去支持下）

对 "WinASAR" 有任何使用上或者技术上的疑问，欢迎随时联系作者。

## 🧧投喂

![Screenshot](https://cdn.jsdelivr.net/gh/flydoos/WinASAR/Images/Donate.png)

## ⚖️免责声明

本程序是作者闲暇之余，为方便自己使用而开发的一个小工具。使用本程序产生的一切后果，需要用户自行承担，作者不承担任何责任！如果对其他人/公司造成不好的影响，请到QQ群联系作者，我会马上删除，谢谢。

<p align="center">
	<img width="100%" src="https://api.star-history.com/svg?repos=flydoos/WinASAR&type=Date"/>
</p>
