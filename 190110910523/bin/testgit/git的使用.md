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

fit                     

![image-20211128164415144](image-20211128164415144.png)

4)push

上传远程代码到远程仓库并合并

前提：远程拥有仓库

![image-20211128170132363](image-20211128170132363.png)

url栏里就是远程仓库地址

先添加远程仓库：

git remote add 别名 远程仓库

![image-20211128172733034](image-20211128172733034.png)



![image-20211128170917278](image-20211128170917278.png)

错误原因：没有指定远程的btanch，需要指定为master

注意：github页面上将master分知名改成了“main”，但push时还是需要用master，master对应页面上的mian

push时命令正确，认证失败：

![image-20211128171453739](image-20211128171453739.png)

获取token的方法：

![image-20211128171702941](image-20211128171702941.png)

点击右上角代表自己的图表，选择settings：

![image-20211128171844523](image-20211128171844523.png)

选择Developer settings：

![image-20211128171930972](image-20211128171930972.png)

选择Personal access tokens:

![image-20211128172034333](image-20211128172034333.png)

点击右侧的蓝色Generate.........:

![image-20211128172439532](image-20211128172439532.png)

点击绿色按钮:

![image-20211128172817538](image-20211128172817538.png)

关闭页面前，需要把token拷贝出来，以后当成密码使用：

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

再次push：![image-20211128173114434](image-20211128173114434.png)

password需要输入token

5）clone

将远程仓库clone到本地：

git clone 远程仓库url

clone后操作步骤：

（1）修改文件

（2）add

（3）commit

（4）远程同步：

分支问题：从本地开始创建的项目，主分支是master；从远程开始，主分支是main。

![](image-20211201165702568.png)

a）添加远程仓库：

git remote add 别名 远程仓库url

![image-20211201172711688](image-20211201172711688.png)

6）diff

查看工作区文件和staging area文件的区别。

![image-20211201173148631](image-20211201173148631.png)

7）查看提交历史log

![image-20211201172736184](image-20211201172736184.png)

8）恢复reset

git reset --hard HEAD^1

回退到上一个版本，--hard将直接修改工作区文件内容。

![image-20211201172840931](image-20211201172840931.png)

## 4.在scode中使用git

1）用命令行进行git初始化

在scode打开项目前，已经执行了git init ，git add





































