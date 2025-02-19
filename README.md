# LionMountainGPT
狮山GPT

~~~markdown
# 项目提交管理仓库

本仓库用于管理其他人的提交，以下是如何在 Windows 系统上使用 Git Bash 拉取和提交代码的详细步骤。

## 1. 克隆仓库

首先，需要将该项目克隆到本地。打开 Git Bash，执行以下命令：

```bash
git clone https://github.com/1071512987/LionMountainGPT.git
~~~

## 2. 查看仓库状态

要查看本地仓库的当前状态，可以使用以下命令：

```bash
git status
```

这将显示文件的修改情况，包括新增、修改或删除的文件。

## 3. 拉取最新代码

在提交代码之前，建议先拉取远程仓库的最新代码，以确保本地代码与远程仓库同步。

```bash
git pull origin main
```

> 如果你的主分支是 `master`，请将 `main` 替换为 `master`。

## 4. 提交代码

### 4.1 添加文件到暂存区

在修改了文件后，使用以下命令将修改添加到暂存区：

```bash
git add .
```

这会将所有修改的文件添加到暂存区。你也可以单独指定文件：

```bash
git add file-name
```

### 4.2 提交更改

然后，提交更改，并附加提交信息：

```bash
git commit -m "你的提交信息"
```

> 提交信息简洁且具有描述性即可，说明你做了哪些修改。

### 4.3 推送到远程仓库

将本地提交推送到 GitHub 远程仓库：

```bash
git push origin main
```

> 如果你的主分支是 `master`，请将 `main` 替换为 `master`。

## 5. 解决冲突

如果在拉取最新代码时发生冲突，你需要手动解决冲突。

Git 会标记出冲突的部分，编辑文件以选择需要保留的内容。解决冲突后，使用以下命令标记为已解决：

```bash
git add file-name
```

然后，继续提交和推送。

## 6. 查看提交历史

可以使用以下命令查看提交历史：

```bash
git log
```

这将显示项目的提交历史，包括每次提交的哈希值、作者、日期以及提交信息。

## 7. 创建新的分支

如果需要在新分支上工作，可以使用以下命令创建并切换到新分支：

```bash
git checkout -b new-branch-name
```

> 使用新分支时，记得在完成工作后合并回主分支。

## 8. 删除本地分支

如果不再需要某个分支，可以使用以下命令删除本地分支：

```bash
git branch -d branch-name
```

> 注意：删除的分支必须已经合并到主分支。
