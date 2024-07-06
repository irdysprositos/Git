# Git常用命令

## 1设置用户签名

Git首次安装必须先设置用户签名，否则无法提交代码

```git
git config --global user.name 用户名
git config --global user.email 邮箱
```

可以在 C 盘，用户中，找到 gitconfig 文件  
可打开查看用户签名配置

****ATTENTION****  
该签名和将来登录的 Github 账号没有关系，只是用来在本地库中标记提交者

## 2初始化本地库

想用 Git 管理一个目录，首先需要 Git 获取管理权限，  
即初始化

```git
git init
```

另查看本地库状态

```git
git status
```

tips:

* vim中 ``yy`` 是复制 ``p`` 是粘贴
* 通用 linux 命令，如：``ll`` 查看目录

## 3新增文件

将文件添加到暂存区

```git
git add xxxx.xxxx
```

将文件从暂存区删除

```git
git rm --cached <file>...
```

## 4提交本地库

将暂存区的文件提交到本地库，形成历史版本

```git
git commit -m "日志信息"
```
