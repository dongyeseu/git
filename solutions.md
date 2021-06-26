# 生成ssh

```bash
ssh-keygen -t rsa -C "邮箱"
```



# 如何查看自己的密钥

```bash
cat ~/.ssh/id_ras.pu
```


# 从本地上传文件到github
```bash
git add ***
git commit -m 'comment' 

git push -u origin main #第一次提交时
git push origin main
```

# 如何将远程仓库的内容同步到本地仓库
```bash
git pull origin

git pull origin master
```



# 如何将远程仓库和本地仓库进行连接

```bash
# 1. git clone 

git clone git@github.com:dongyeseu/LeetCode.git 

# 2. git remote add origin 
git init 
git remote add origin git@github.com:dongyeseu/LeetCode.git
```



# 命令行中出现END如何退出

**按q键**



# 如何设置签名

```bash
# 项目级别/仓库级别： 仅在当前本地库范围内有效
git config user.name [name]
git config user.email [email]

# 系统用户级别： 登陆当前操作系统的用户范围
git config --global user.name [name]
git config --global user.email [email]

# 优先级
1） 项目级别 高于 系统用户级别
2） 如果没有项目级别，则使用系统用户级别
```



# 如何查看历史记录并回退版本

```bash
# 查看历史版本
git log 

git reflog

git log pretty=oneline

# 回退到某个版本
# 基于所引致操作
git reset --hard [版本哈希值]  
e.g. git reset --hard efddb97

# 基于^，表示后退; 一个^代表后退一步
git reset --hard HEAD^^^  

# 基于~,表示后退;~后面的数字代表后退的步数
git reset --hard HEAD~3
```

