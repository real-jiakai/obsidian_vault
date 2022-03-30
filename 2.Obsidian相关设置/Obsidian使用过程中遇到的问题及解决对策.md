#obsidian 

## 1.BiliBili视频内嵌

在obsidian中内嵌入BiliBili视频时，显示空白。解决对策，见中文论坛的这个[帖子](https://forum-zh.obsidian.md/t/topic/594)，在iframe标签的src属性前添加`https:`即可解决问题。

## 2.PDF导出

安装了Pandoc插件，ctrl+p打开命令面板，输入pandoc，发现没有导出pdf的选项，后来在网上查阅资料后解决了该问题，Obsidian右上角自带导出pdf功能。

![](https://vip1.loli.io/2022/03/28/zG2eyKWxwDJLS8g.png)

## 3.Git同步

使用Obsidian Git插件同步简便操作，可以看这篇[文章](https://publish.obsidian.md/chinesehelp/01+2021%E6%96%B0%E6%95%99%E7%A8%8B/obsidian%E5%92%8CGit%E8%BF%9E%E7%94%A8%E5%AE%9E%E7%8E%B0%E7%89%88%E6%9C%AC%E6%8E%A7%E5%88%B6%EF%BC%88obsidian+Git%E6%8F%92%E4%BB%B6%E4%BB%8B%E7%BB%8D%EF%BC%89+by+%E8%BD%AF%E9%80%9A%E8%BE%BE)。

我使用此插件后觉得不合适，所以我主要使用windows下的任务计划程序来完成每天的备份。我的.bat文件的内容如下：

```shell
d:
cd D:\obsidian_vault
git add .
git commit -m "auto deploy"
git push --force
```

每天的21:00任务会自动进行。

后序补充：

后来，我想将ipad端的obsidian和windows端通过icloud云盘同步【具体可见官方的[同步教程](https://help.obsidian.md/Getting+started/Sync+your+notes+across+devices)】，并每天定期将windows下的icloud云盘中的obsidian vault下的内容推送到github。我就改写了.bat文件的内容。如下：

```shell
cd C:\Users\Gu Jiakai\iCloudDrive\iCloud~md~obsidian\obsidian_vault
git add .
git commit -m "auto deploy"
# git push origin master --force
git push --force
```

这其中我遇到了一个问题，GitHub创建仓库，并将其克隆下来，然后将obsidian的vault中的文件移至克隆下来的空仓库中，git push提交上去的是GitHub的main分支。

我一开始使用shell脚本，push的时候在远端新建了一个master分支，并提交至该分支【git push origin master --force】，因此当我查看github仓库的时候发现，有一个main分支，还有一个master分支。最后，我修改了GitHub上该仓库的默认分支为master分支，将原本的main分支删除。这样，Obsidian的icloud同步和GitHub备份就两全了。

## 4.Obsidian写作插入表情

一开始我写作一直以来用Markdown表情短代码来插入表情【如`:smile:`=😄，，但是这在Obsidian Publish上就不奏效了。如果Obsidian软件不装表情短代码插件的话，也不会支持这样的操作。

后来在Obsidian官方群里面，外国网友解答了我的疑惑。windows电脑用`win+.`，可以实现表情的插入，注意这边的`.`，是键盘上问号旁边的按键，并非小键盘的按键。这是Windows电脑的自带的表情符号，在任何地方通用的。如写html文件的时候想插入表情，即可通过此快捷键实现。

## 5.Obsidian打开大纲视图

设置—核心插件—大纲，开启，即可在大纲视图。