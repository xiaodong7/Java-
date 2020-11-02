### **GitHub 学习指南   2020.11.01**

[toc]









#### 一、配置

```java
git config --global user.name "xiaodong7"             #用户名
git config --global user.email "1902458823@qq.com"     #邮箱
# 查看信息
git config -l  
```



#### Vim 常见的命令

1. 'i'进入编辑模式
2. 'esc'进入命令模式
3. ':wq'保存退出
4. 'q!'不保存强制退出

**二、常用命令**

```
 提交流程
 git add document.txt   #将工作区文件添加到暂存区

 git commit -m "first commit"  #将暂存区文件添加到本地仓库
 
 git push origin Document      # 将当前分支提交到远程Document 分支
 
 git pull origin Document      #下载远程分支Document 代码
 
 本地目录修改文件后，必须add  commit push
从工作区 --> 暂存区 --> 本地仓库 --> 远程仓库

 git merge Document           # 合并指定Document分支到当前(main)分支
 
 
 #克隆远程仓库  在任何文件目录
 git clone git@github.com:xiaodong7/GitHubTest.git

```



```
git init   #创建新的版本库  在某一目录下  git bash
```



如果一开始远程克隆仓库无法下载，发生超时，在Git\etc\ssh下config文件下末尾添加以下代码

```
Host github.com
User 1902458823@qq.com
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa
Port 443
```



```java
#克隆远程仓库  在任何文件目录
 git clone git@github.com:xiaodong7/GitHubTest.git

#新建一个分支
git branch [branch-name] 

#切换到指定分支
git checkout [branch-name] 

```

**分支**

```markdown
#列出所有本地分支
git branch

#列出所有远程分支
git branch -r 

#列出所有本地、远程分支
git branch -a 

#新建一个分支
git branch [branch-name] 

#新建一个分支，并切换到该分支
git checkout -b [branch] 

#切换到指定分支
git checkout [branch-name] 

#合并指定分支到当前分支
git merge [branch] 

#
git rebase [branch]

#删除分支
git branch -d [branch-name]

#删除远程分支
git push origin --delete [xiaodong7-测试文件夹] 

#删除远程分支
git branch -dr [remote/xiaodong7-测试文件夹]
```















