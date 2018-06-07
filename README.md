# git
git information
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

