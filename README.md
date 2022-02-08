# learn_lazygit

我使用这个仓库来学习 lazygit,我会在这里来测试 lazygit 的命令

## 我需要学习的东西 (目前)

- 学会如何用 lazygit 来删除分支
- 学会如何用 lazygit 来建立多个分支,多个开发
-

## 全区快捷键

- 按(z)快捷键 撤销

## 目前已经学习到的东西(按照分区进行划分(lazygit 中的 12345 这五个分区加划分))

### git 暂存区显示和操作(第二分区)操作

- 按(a)快捷键可以快速的把所有文件 staged
- 按(A)快捷键可以将现在这次文件(**选中的文件**)合并到上个没有提交(push)的修改
- 按(e)快捷键来用 nvim 来编辑那个文件

### git 分支区显示和操作(第三分区)操作

- 按(n)快捷键能够快速建立分区
- 按(R)快捷键能够快速重命名分区

### git 提交和日志(reflog)区显示和操作(第四分区)操作

- 按(r)快捷键可以把提交改名(push)到远程库的也能改名,改名完后再 push 到远程库就修改成功了
- 按(g)快捷键可以重置提交 然后这里会有选项 (soft mixed hard)
- 按(s)快捷键可以压缩提交,可以压缩当前文件下面的第一个 commit(**只能有一个**)

## git 回滚的相关知识

这里 git 回滚主要有下面三个命令

- git reset--soft
- git reset--mixed
- git reset--hard

### 已经提交,没有 push

1. git reset --soft 撤销 commit
2. git reset --mixed 撤销 commit 和 add 两个动作

### 已经提交,并且 push 了

1. git reset --hard 撤销并舍弃版本号之后的提交记录.**使用需要谨慎**
2. git revert 撤销,但是保留提交记录

**记得把 插入模式的 lazygit(快捷键) 移除**
