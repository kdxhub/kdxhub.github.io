---
title: "u2lock"
---
<small><a href="/">首页</a> | <a href="/blogs">Blogs</a> | <a href="/Project">项目合集</a> | <a href="https://space.bilibili.com/1987247870">Bilibili↗</a><br><a href="../">←返回</a> |
 创建：2023-03-05 | 最后更新：2023-03-05</small><br>

# [宣传片](https://www.bilibili.com/video/BV1so4y1q7Ft/)

# 起因
看了某个引流号的视频突发奇想做个颜值更高且没有套路的U盘锁屏软件

# 原理
通过检测指定目录的文件所含**私钥**是否与本地**公钥**相吻合。<br>
若不吻合则弹出自绘锁屏页面，并持续进行上述检查，直到吻合。<br>
加密算法：`SHA256`<br>

# 兼容平台
理论上Windows XP→11都支持

为了防止手贱把U盘搞不见了、配置文件乱改一通完全识别不了，**此时可以右键锁屏，来使用Windows锁屏解锁，并且软件自动退出**<br>
# [下载](./path)