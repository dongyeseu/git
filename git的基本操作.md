

# 1. 基本操作

```bash
# 状态查看操作 : 查看工作区、暂存区的状态
git status
```



```bash
# 添加操作 : 将工作区的“新建/修改“添加到暂存区
git add [file name] 
```



```bash
# 提交操作： 将暂存区的内容提交到本地库
git commit -m "commit message" [file name]
```



```bash
# 查看历史记录
git log 

git reflog

git log pretty=oneline
```



```bash
# 版本回退
git reset --hard [版本哈希值]

git reset --hard HEAD~1

git reset --hard HEAD^
```



```bash
#比较文件差异
git diff [文件名]  # 是将工作区的文件和暂存区的文件进行比较
git diff [本地库中历史版本][文件名] # 是将工作区中的文件和本地库中的历史记录进行比较
```

