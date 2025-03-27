# 得到一个 git repo<sup>仓库</sup>

这里没有 “鸡生蛋”/“蛋生鸡” 的困惑, 想要用 git 来做版本管理, 首先你得有一个 git repo

两种方式 新建一个<sup>`git init`</sup> 或者 拿来主义<sup>`git clone`</sup>

## 新建

1. 准备一个空文件夹

2. 如果你是 **Linux**/**MacOS**, 使用 **终端工具** 切换到该文件夹
   ```shell
   $ cd /Here/Is/Your/Empty/Dir
   ```

   如果你是 **Windows**, 当然你也可以按上面的方式来, 使用 CMD 或者 PowerShell, 我个人更习惯使用 **文件浏览器** 打开准备好的空文件夹, **右键** -> **Open Git Bash Here**

3. 使用命令 `git init` 完成仓库初始化

## 克隆

克隆则是把已有的 git repo 在你本地创建一个副本

1. 切换到你准备存放该仓库的文件夹
   同上面 **新建 步骤2** 类似, 我们需要进入到一个文件夹
2. 使用 `git clone https://Here-Is-The-Git-URL [你可以指定克隆后的文件夹名]` 