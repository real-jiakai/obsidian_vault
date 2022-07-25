- 归档：[[Obsidian]]
---


#Obsidian

## Obsidian Publish的相关配置

1.在vault中新建的publish.css文件可以参考这个仓库-[obsidian-publish-css](https://github.com/selfire1/obsidian-publish-css)。该仓库的作者的笔记被obsidian官方选做了展览馆中的范例站点。

> [!note]
> 2022年的4月4号，更换了publish.css样式文件。主要参考了这个[css文件](https://publish-01.obsidian.md/access/3c4cf261765d1b812b962974f8d190ab/publish.css)。
> 
> 其实每个Obsidian Publish的站点的样式文件可以在浏览器的"F12+网络"中获取。

2.关于如何使得Obsidian Publish支持markdown的扩展表情语法，即通过书写短代码实现表情，需要自己编写publish.js。由于本人水平有限，无法实现此功能。
代替的做法：windows电脑，按住win键，再按住英文输入法下的`.`(逗号旁的点)，使用windows自带的表情。再次发布，即可看到表情正常显示。我的这篇笔记【[[Obsidian使用过程中遇到的问题及解决对策]]】中有提及。

3.Obsidian Publish图片放大，可以参考[此博文](https://publish.obsidian.md/maolaoda/%E5%AD%A6%E4%B9%A0/%E7%AC%94%E8%AE%B0%E8%BD%AF%E4%BB%B6/Obsidian%E9%85%8D%E7%BD%AE#11+%E7%85%A7%E7%89%87%E7%82%B9%E5%87%BB%E6%94%BE%E5%A4%A7)

4.Obsidian Publish如何隐藏底部的`Powered by Obsidian Publish`，可以在publish.css中加入以下代码实现。个人认为没必要隐藏。

```css
.site-footer{
	display:none;
}
```

5.Obsidian Publish很方便，但是也很贵。如果你对其感兴趣的话，请量力而行。

6.关于标注块，Obsidian已经原生支持，不需要额外的配置。可以装个Admonition插件来方便自己的插入操作。具体可见，我的这篇日记【[[2022-03-29]]】

![](media/Ki1N5Ec7XrkLeJa.png)

