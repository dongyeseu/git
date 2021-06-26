

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



```bash
# 创建分支
git branch [分支名]

# 查看分支
git branch -v

# 切换分支 
git checkout [分支名]

# 如何将分支的内容合并到master上
git checkout [分支名]
git add [file]
git commit -m "comment"
git push --set-upstream origin [分支名]
git checkout master
git merge [分支名]
git push origin mains
```



```bash
git branch
1、切换到某分支　　git checkout branchName
2、创建某分支　　git branch branchName
3、查看本地所有分支　　git branch
4、查看远程所有分支　　git branch -r
5、查看本地和远程所有分支　　git branch -a
6、删除本地分支　　git branch -d branchName
7、删除远程分支　　git push origin :branchName　　(":"代表删除)
9、重命名　　git branch -m oldName newName

```



```bash
pull = fetch + merge 
git fetch [远程库地址别名][远程分支名]
git merge [远程库地址别名]/远程分支名]
```





