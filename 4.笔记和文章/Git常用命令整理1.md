#Git

```bash
# 创建一个空的Git存储库或重新初始化一个现有的存储库。
git init
# 查看项目的状态。 
git status
# 查看项目的简要信息
# s是short的缩写
git status -s
# 显示项目的详细信息
# v是verbose的缩写
git status -v
# 把工作区的所有变化提交到暂存区。
git add .
# 显示暂存区和工作区的差异。
git diff 
# 显示工作区与当前分支最新提交之间的差异。
git diff HEAD
# --cached和--staged效果一样
# 显示暂存区和上一个提交至版本库内容的差异。
git diff --cached
# 显示暂存区和上一个提交至版本库内容的差异。
git diff --staged
# 将暂存区内容添加到版本库，-m选项用以在命令行中提供提交注释。 
# m为message的缩写。
git commit -m "xxx"
# 跳过将已追踪过的工作区文件添加至暂存区的流程，直接提交到版本库。 
# 注：未被追踪过的工作区文件，无法实现一键提交至版本库！
git commit -am "xxx"
# 修改上一条提交信息。
git commit --amend
```