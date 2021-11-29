# git的使用

## 1.git的安装

使用库安装：

sudo apt update

sudo apt-get install git

测试：git --version

## 2.git的概念和工作流程

![image-20211124172551617](image-20211124172551617.png)

![image-20211128162955737](image-20211128162955737.png)

## 3.git常用命令

1）git项目创建

创建一个目录，在此目录下执行 git init

执行后，会创建一个隐藏的.git

![image-20211124173129404](image-20211124173129404.png)

2）

![image-20211128162921564](image-20211128162921564.png)

3）commit

提交文件到本地库

提交所有在staging area中的文件到registory：

git connit -m[message]

message是提交时的备注

![image-20211128163353848](image-20211128163353848.png)                              

![image-20211128164415144](image-20211128164415144.png)

4)push

上传远程代码到远程仓库并合并

前提：远程拥有仓库

![image-20211128170132363](image-20211128170132363.png)

url栏里就是远程仓库地址

先添加远程仓库：

git remote add 别名 远程仓库