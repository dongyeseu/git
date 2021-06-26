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

git remote add origin git@github.com:dongyeseu/LeetCode.git
```



# 命令行中出现END如何退出

**按q键**



# 如何设置签名

```bash
# 项目级别/仓库级别： 仅在当前本地库范围内有效
git config user.name 
git config user.email 

# 系统用户级别： 登陆当前操作系统的用户范围
git config --global user.name 
git config --global user.email
```

