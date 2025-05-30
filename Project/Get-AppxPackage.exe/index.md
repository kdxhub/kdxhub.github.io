---
title: "Get-AppxPackage 软件包安装程序の平替"
description: "Get-AppxPackage"
---
<small id="old_menu"><a href="/">首页</a> | <a href="/blogs">Blogs</a> | <a href="/Project">项目合集</a> | <a href="https://space.bilibili.com/1987247870">Bilibili↗</a><br><a href="../">←返回</a> |
 创建：2023-02-28 | 最后更新：2025-02-14</small><br>

<big>[视频介绍](http://b23.tv/BV1VA411z7bq)</big> | <big>[制作语言包教程](./how-to-make-lang-profile)</big><br>
![](https://s1.ax1x.com/2023/02/28/ppCUGuT.png "All-v3;in-v1.1.0.0")

## 一、为什么作者要使用“Get-AppxPackage”而不是“Add-AppxPackage”来作为标题（114分）
答：用来讽刺Windows的诸多BUG
## 二、试分析其的实质（514分）
答：PowerShell套壳
## 三、给作者三连（1919810分）
（开放性试题，意对即可）

# 下载 Download

<big><b>↓ 这个“主程序”可以点击！！ ↓</b></big>
 
|文件|SHA256校验|
|:-:|:-|
| **点它！→**[主程序฿](https://rs.kdxiaoyi.top/res/projects/Get-AppxPackage/Get-AppxPackage.exe) | `e878bd09aab73c54a4a17fc207fcbf9d478e67bafc14056a91dd766684273b9c` |
| [源代码฿](https://rs.kdxiaoyi.top/res/projects/Get-AppxPackage/Get-AppxPackage.e) | `f249d82609b996ddf7fac970ec2c695a7abe9bfdf69e553fca580e74d690e5ed` |
| [应用图标฿](https://rs.kdxiaoyi.top/res/projects/Get-AppxPackage/Get-AppxPackage.ico) | `5c57a54e37b2490b8b899196e808fd7bff913c254354939ecfdc2f8356851658` |

# 大致原理
根据用户的配置生成Powershell脚本并执行<br>
当然为了保证运行效率，实际采用`cmd.exe /c powershell`的方式

# 兼容平台
Windows 10+<br>
Windows 8……应该能用？ <sup><a target="_blank" href="https://www.404techsupport.com/2014/06/23/installing-free-windows-8-modern-apps-without-the-windows-store/">[信息来源在这里]</a></sup><br>

**需要启用“旁加载”模式**。关于如何启用，请参阅[Microsoft Learn](https://learn.microsoft.com/zh-cn/windows/application-management/sideload-apps-in-windows-10#step-1-turn-on-sideloading)。<br>
Windows10+的省流：[点我打开设置](ms-settings:developers)，勾上“开发人员模式”或“从任意源（包括松散文件）安装应用”<br>

# 兼容性
~~我知道有什么多语言支持，但在我这套源码的基础上改个语言包不是什么难事，微软的多语言也是外置包.mui搞得  ←23-02-23-Updata:**已经支持多语言**<br>
另外，我这套UI本质基于Win32UI，UI兼容性微软已经替我考虑了。

# Updata Log
## 下一步计划
- 修复任意拖动功能失效、文件名被吞的BUG
- 新增`Winget`相关支持

## 总v3；v1.1.0.1
- 更新多语言

## 总v3；v1.1.0.0
- 现在兼容4种由微软文档给出的软件包格式（Appx/Msix/Appxbundle/Msixbundle）
- 可选是否启用强制安装模式、是否启用日志模式
- 新增了右键菜单
- 现在会显示软件包的文件名
- 现在可以重新打开选包界面
- 现在会把使用的命令行输出到文件（./cmdLine）内，且每次都会覆盖上次写入

已知BUG:
- 若打开的包格式不正确，它的文件名会被吞（由于编辑框控件的缺陷导致）
- 右键菜单并不能全局生效（事件没有注册到标签控件上）
- 任意拖动功能失效（忘开了）

## 总v2；v1.0.0.0
第一个Public version，很热乎呢~

<script src="https://rs.kdxiaoyi.top/res/scripts/js/sober@1.0.6.min.js"></script><script src="https://kdxiaoyi.top/pmd.js"></script><script src="https://rs.kdxiaoyi.top/res/scripts/js/pmd-reRender.min.js"></script>