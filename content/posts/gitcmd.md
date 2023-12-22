+++
title = 'git常用命令'
date = 2023-12-20T22:30:32+08:00
draft = false
tags = ["git"]
categories = [""]
+++



Git上传文件到Github(最详细)
大致步骤
本地仓库：

a. git init 在本地创建一个Git仓库；

b. git add . 将项目添加到暂存区；

c. git commit -m "注释内容" 将项目提交到Git仓库；

远程仓库：

a. 添加SSH KEY；

b. 新建repositories；

本地仓库：

a. git remote add origin git@github.com:UserName/projectName.git 将本地仓库与远程仓库关联；

b. git push -u origin master/main 将本地项目推送到远程仓库。



git pull origin main // 把本地仓库的变化连接到远程仓库主分支   //理解是上传本地文件到远程仓库
git branch -M main //选择main分支，可以改名上传其它分支

git clone https://github.com/festalstar/hugo_blog.git


OpenSSL SSL_connect: Connection was reset in connection to github.com:443
#修改 Git 的网络设置
git config --global http.proxy http://127.0.0.1:7890 
git config --global https.proxy http://127.0.0.1:7890

 取消代理
git config --global --unset http.proxy
git config --global --unset https.proxy

 查看代理
git config --global --get http.proxy
git config --global --get https.proxy

git config --global http.sslVerify false