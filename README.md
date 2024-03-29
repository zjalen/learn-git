# Learn How to Use Git
## 学习如何使用 Git 命令
[Git 实例指南（一）介绍安装](https://www.jalen.top/#/cate/5/article/26)

### Step 1

```bash
git init # 初始化一个版本库
git add -A . # 添加所有文件到暂存区
git status # 查看当前版本库的状态
git commit -m "备注" # 提交到本地库
git remote add origin git@github.com:zjalen/learn-git.git # 关联线上版本
git push -u origin master # 首次推送到线上
git clone # 直接从线上克隆到本地。
```

### Step 2

```bash
git reset HEAD <文件名>  # 撤销文件的暂存
git checkout -- <文件>  # 丢弃工作区的改动
git log # 查看版本历史，参数 --pretty=oneline 精简显示
git reflog # 查看所有分支历史
git reset --hard <版本号> # 回到指定版本，版本号或者 HEAD 指针位置
git push # 推送到远程库
git clone <远程地址> # 克隆远程库到本地
```

### Step 3

```bash
git branch <分支名>  # 创建分支
git checkout <分支名> # 切换分支
git branch  # 查看分支
git merge <分支名>  # 把指定分支内容合并到当前分支
git push origin dev  # 将本地 dev 分支上传到线上仓库
git pull # 从线上同步到本地
git log --graph --pretty=oneline --abbrev-commit  # 显示 ASCII 图形表示的分支合并历史 --graph 显示 ASCII 图形表示的分支合并历史 --pretty=oneline  优化显示效果 --abbrev-commit 显示部分版本号而非全部
git rebase  # 变基操作
```

### Step 4

```bash
git tag <标签>  # 添加标签
git tag -d <标签号>  # 删除标签
git tag -a <标签> -m "备注" <版本号>  # 指定版本号标签与备注
git show <标签> # 查看更多标签信息
git push origin <标签>  # 推送某一个标签
git stash  # 使用 stash 命令进行保存
git stash list # 查看 stash 列表
git stash apply  # 应用恢复 stash
git stash apply stash@{n} # 应用恢复指定版本 stash
git stash drop  # 删除缓存的 stash
git stash pop # 应的同时删除
```
