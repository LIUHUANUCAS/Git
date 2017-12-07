# git的使用方法小结

## 1.git 创建本地分支

### 1.1 在本地创建分支

```git
    git branch branch_name  //创建本地分支
    git checkout branch_name //切换分支
```

- 可以使用如下命令创建并切换分支

```git
    git checkout -b branch-name //创建本地分支,并切换到新分支上
```

### 1.2 在本地创建分支 关联本地分支和远程分支

```git
    git push origin branch_name:remote_branchname //
    git branch --set-upstream-to=origin/remote_branch_name  branch_name 关联本地和远程的分支
```

### 1.3 从其他分支拉取自己的分支步骤

```git
    1.git checkout remote_branch
    2.git branch yourlocal_branch
    3.git checkout  yourlocal_branch
    4.git push origin yourlocal_branch:remote_branch
    5.git branch --set-upstream-to=origin/remote_branch yourlocal_branch
```
