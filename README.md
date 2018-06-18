# git

## git本地操作
- 不停的创造文件进行备份(没有修改的提示) git可以帮我们管理我们的代码保证代码不丢失
- 记录历史只要代码提交到git上就永久不会丢失，可以随时“穿越”
- 团队协作 俩个人修改了同一个文件的同一行，也需要手动解决冲突，可以实现自动合并 （模块化，组件化）
- git拥有强大“分支”管理系统

## 分布式
- svn(集中式) 需要一台中央服务器

## git的区别
- 速度比svn快
- svn中每个文件夹都有一个文件.svn文件，git有一个单独的文件.git文件夹

## git安装
- windows http://git-scm.com
- mac 如果安装过xcode自带git，homebrew是wmac的包管理器
- http://ohmyz.sh/
- http://www.iterm2.com/

## 配置用户(不配置用户不能提交代码)
```
git config --list
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

## 初始化git
一个项目初始化一次，不能嵌套
```
git init 告诉git哪个文件夹被git所管理
git status 查看git状态
```

## 删除暂存区
```
git rm --cached 文件名
```

## 添加到暂存区
```
git add ./ -A / 文件名
```

## 添加到历史区
```
git commit -m '消息'
```

## git的对比
git diff 工作区和暂存区
git diff 分支名 工作区和历史区
git diff --cached 暂存取和历史区比较

## 撤销
```
从暂存区中将工作区内容覆盖掉
git checkout 文件名
git reset HEAD 文件名 回到上一次的缓存区
```

## 回滚历史版本
```
git reset --hard 版本号
git reflog 查看所有版本
```

## 回滚某个版本的文件
```
git checkout 版本号 文件名
```

## 创建分支
```
git branch 分支名
```

## 查看分支
```
git branch
```

## 切换分支
```
git checkout 分支名
```

## 删除分支
```
git branch -D 分支名
```
> 删除分支时，当前用户不能在当前要删除的分支上

## 创建并切换分支
```
git checkout -b 分支名
```

## 文件修改切换分支
```
git stash
暂存文件
git stashpop
还原暂存的内容
```
> 分支有修改不能直接切换，可以提交更改或暂存更改,过渡区覆盖工作区

## 合并分支
```
git merge 分支名
```

## 日志
```
git log 日志
git log --graph 日志图标
git log --graph --online 简化图标
```

## 关联远程仓库／推到github
- 本地新建项目
- git init
- 添加README.MD 和 .gitignore
- 提交到版本库
- git remote add origin github地址
- git push -u origin master   (第一次push加 -u ，之后自动默认提交到该分支里)

## 删除关联
```
git remote rm 名(origin)
```

 > .gitignore 忽略提交内容的隐藏文件

 > git 不会上传空文件夹 添加.gitkeep保存空文件夹

## linux命令
- pwd print working directory
- rm -rf 文件夹 删除文件
- rm 文件名 删除文件
- mkdir 文件夹名字 创建目录
- cd 目录名 change directory
- ls -al显示目录下所有的文件
- touch 文件名 创建文件
- cat 文件名


