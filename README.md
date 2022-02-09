# 学习使用 lazygit

我使用这个仓库来学习 lazygit,我会在这里来测试 lazygit 的命令

## 我需要学习的东西 (目前)

- [x] 学会分支的基本操作 (删除,新建,合并)
- [x] 学会如何回退代码(并在远程仓库也体现出来)
- [x] 学会如何合并代码(先选择\*分支,然后再选择分支 M 键 merge)

## 全局快捷键 (个人常用)

- 按(p)pull 把远程代码拉到本地
- 按(P)push 把本地代码 push 到远程库
- 按(z)快捷键 撤销
- 按(ctrl-d)快捷键 可以在 diff 窗口向下滚动 (查看 diff 好用)
- 按(ctrl-u)快捷键 可以在 diff 窗口向上滚动 (查看 diff 好用)
- 按(,)快捷键 可以在分区选择窗口向上翻页
- 按(.)快捷键 可以在分区选择窗口向下翻页

## 目前已经学习到的东西(按照分区进行划分(lazygit 中的 12345 这五个分区加划分))

### git 状态去(第一分区)

这个分区目前的功能就是显示你的状态.
后面我会完善状态的介绍

### git 暂存区(第二分区)

- 按(a)快捷键可以快速的把所有文件 staged
- 按(A)快捷键可以将现在这次文件(**选中的文件**)合并到上个没有提交(push)的修改
- 按(e)快捷键来用 nvim 来编辑那个文件

### git 分支区(第三分区)

- 按(n)快捷键能够快速建立分区
- 按(R)快捷键能够快速重命名分区

### git 提交和日志(reflog)区(第四分区)

- 按(r)快捷键可以把提交改名(push)到远程库的也能改名,改名完后再 push 到远程库就修改成功了
- 按(g)快捷键可以重置提交 然后这里会有选项 (soft mixed hard)
- 按(s)快捷键可以压缩提交,可以压缩当前文件下面的第一个 commit(**只能有一个**)

### git 封存(stash)区

## git cherry-pick(遴选)

在使用 lazygit 的时候发现有 git cherry-pick 这个命令,但是我却不知道这个是什么含义,于是 google 了下,了解其中的含义

> 当你和一群程序员一起工作时，无论项目大小，处理多个 Git 分支之间的变更都会变得很困难。有时，你不想将整个 Git 分支合并到另一个分支，而是想选择并移动几个特定的提交。这个过程被称为 “遴选 cherry-pick”。

### Reference

[什么是 Git 遴选](https://linux.cn/article-13295-1.html)

## git 回滚的相关知识

这里 git 回滚主要有下面三个命令

- git reset--soft
- git reset--mixed
- git reset--hard

### 已经提交,没有 push

1. git reset --soft 撤销 commit
2. git reset --mixed 撤销 commit 和 add 两个动作
3. git reset --hard 回到那次提交 commit 和 add 全部不留

### 已经提交,并且 push 了

1. git reset --hard 撤销并舍弃版本号之后的提交记录.**使用需要谨慎**
2. git revert 撤销,但是保留提交记录

## 最近要做的事

- 使用并了解 neorg
- 修改 prettier 格式化属性
