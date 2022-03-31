#GitHub #个人主页

# GitHub主页实现svg图片动态效果

众所周知，在GitHub上新建一个与自己用户名相同的仓库，该仓库中的README.md文件会在GitHub的个人主页进行展示。

详情请[click me。](https://docs.github.com/cn/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)

但是，在不经意间，我看到了GitHub用户名为[MayanDev](https://github.com/Mayandev)大哥的个人主页酷炫的动态打招呼特效。

具体请见以下动态gif图片。👇

![2022031201.gif]( https://cdn.gujiakai.top/image/pic-go-typora02/img/202203121243311.gif)

非常炫酷，点击动态打招呼特效，会跳转到一个专门生成手写字的[网站](https://www.calligrapher.ai/)

![2022031202]( https://cdn.gujiakai.top/image/pic-go-typora02/img/202203121248273.gif)

可以点击左上角的下载图标，将刚才手写字下载下来。

下载下来是一个后缀为svg的文件。

> what is svg file?

可缩放矢量图形（英语：Scalable Vector Graphics，缩写：SVG）是一种基于可扩展标记语言（XML），用于描述二维矢量图形的图形格式。SVG由W3C制定，是一个开放标准。

双击下载下来的以svg为后缀的文件，在浏览器打开，发现其并没有一开始网站上的动态效果。

![image-20220312125513098]( https://cdn.gujiakai.top/image/pic-go-typora02/img/202203121255238.png)

> How to  make svg file dynamic?

关于这个问题，我特意询问了[MayanDev](https://github.com/Mayandev)。

这是我和他的邮件交流记录。👉[click me](https://qiniuyun.gujiakai.top/pdf/blog/github-email.pdf)

> Summary：

+ 将刚才下载下来的svg图片用代码编辑器打开。
+ 整理格式(删减不需要的内容)。
+ 在开头加一段css代码。
+ 将svg文件用markdown语法的超链接语法展示

> 用代码编辑器编辑前的svg文件和编辑后的svg文件的区别，见以下超链接。

[click me](https://github.com/Jaya0455/Jaya0455/commit/bc3ff7305807b7e4e064e9207e3775ace5ad80d8?diff=split)