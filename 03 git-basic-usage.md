# `git status`

用来查看本地 git repo 目前状态

```shell
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        00 git-install.md
        01 pre-config.md
        02 get-a-repo.md
        README.md

nothing added to commit but untracked files present (use "git add" to track)
```



# `git add`

把文件提交 **暂存**, 这个操作会把 **untracked** 的文件提交给 git repo, 告诉它 "请帮我做该文件的版本管控"

```shell
$ git add .
# 这步是告诉 git 当前文件夹(.) 下面所有 untracked 的文件都需要纳入版本控制

# status 可以看到 git 已经知道下一次提交时需要加上哪些文件了
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   00 git-install.md
        new file:   01 pre-config.md
        new file:   02 get-a-repo.md
        new file:   README.md

```



# `git commit`

做一次提交, 意即你的 git repo 会做一次版本的更新了

```shell
$ git commit
# 会立即进入下面的画面, 让用户编辑本次提交的信息

# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
#
# On branch master
#
# Initial commit
#
# Changes to be committed:
#       new file:   00 git-install.md
#       new file:   01 pre-config.md
#       new file:   02 get-a-repo.md
#       new file:   README.md
#
## 在这里你可以写上你对于本次提交的备注
```



写完保存, 得到如下输出

```shell
[master (root-commit) 5b938fe] First commit, some git basic knowledge
 4 files changed, 73 insertions(+)
 create mode 100644 00 git-install.md
 create mode 100644 01 pre-config.md
 create mode 100644 02 get-a-repo.md
 create mode 100644 README.md
```



# `git remote`

用来管理远程仓库

```shell
# 添加一个远程仓库, 本地别名为 demo
git remote add demo https://HERE-IS-THE-REMOTE-REPO-URL

# 查看当前 git repo 关联的 remote
# 可以带上 -v
git remote
```



# `git fetch`

获取仓库内容

```shell
git fetch demo
```



# `git push`

将本地 repo 的 commit 与远程同步



# `git pull`

等效于 `git fetch` + `git merge`<sup> *merge* 是 **分支合并** 操作</sup>

