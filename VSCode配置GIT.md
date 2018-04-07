# VSCode配置GIT流程
### 1 下载并安装git
### 2 建立一个需要同步的文件夹，在该文件夹内运行git bash 
#### 2.1 git全局配置
    git config --global user.name "yourname" 
    git config --global user.email "youremail@qq.com"
#### 2.2 初始化git目录
    git init
### 3 在github上新建仓库
### 4 在刚才建立的需要同步的文件夹中运行git bash
#### 4.1 添加需要同步的文件，提交，并第一次推送到远程github上
    git add [增加到缓存区的文件]
    git commit -m "提交备注"
    git remote add origin [远程仓库链接]
    git push -u origin master
#### 4.2 以后每次本地提交后如果需要推送到远程github上
    git push origin master //推送master分支
### 5 用VSCode打开刚才建立的文件夹，在源代码管理模块中可以查看到git操作界面
![vscode源代码管理器界面](/源代码管理器界面.PNG)