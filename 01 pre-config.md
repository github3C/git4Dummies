# 添加用户信息

在使用git做版本管理前, 你需要告诉git: “你是谁”

```shell
git config --global user.name "Linus"
git config --global user.email "linus@git.org"
```

> 这里的信息只是用来关联你的提交, 所以你可以不按实际信息来写
>
> 导致后果则为别人无法通过这些信息找到你<sup> 很脱裤子放屁, 是吧?</sup>

上面的命令会把你的信息写到 *~/.gitconfig* 文件

在 Windows 系统下的话, 应该是当前登录用户的用户文件夹下

## git 的配置文件

git 其实会有很多个 config 文件

上面提到的命令使用 `--global` 写入了 **用户全局** 配置文件, 它会对 **系统当前登录用户** 生效<sup> 如果你没有配置其它更细致的 config 的话</sup>

更高层级还有 `--system` 对 **本计算机上所有的用户** 生效

更低层级则有 `--local` 对 所在 **git repo<sup> 仓库</sup>** 生效



# 拓展知识

当你需要使用帮助时, 首先可用的是 `git -h`, 它会给你列出 git 的常见命令

> 'git help -a' and 'git help -g' list available subcommands and some
> concept guides. See 'git help <command>' or 'git help <concept>'
> to read about a specific subcommand or concept.
> See 'git help git' for an overview of the system.

当然, 列在 **00 文档** 中的 **官方在线手册** 也是可以用的

还没有解决方法? 那就去求助 **搜索引擎** 吧!