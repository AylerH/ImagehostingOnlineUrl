# 概览-PicGo: 一个用于快速上传图片并获取图片 URL 链接的工具
[github：包含picgo图床软件](https://github.com/Molunerfinn/PicGo/)
图片上传位置github项目：https://github.com/AylerH/ImagehostingOnlineUrl
PicGo 本体支持如下图床(免费可使用github)：
```
七牛图床 v1.0
腾讯云 COS v4\v5 版本 v1.1 & v1.5.0
又拍云 v1.2.0
GitHub v1.5.0
SM.MS V2 v2.3.0-beta.0
阿里云 OSS v1.6.0
Imgur v1.6.0
```
# picgo使用github作为默认图床-使用方法
## 获取github token
## 在 GitHub 上获取 Personal Access Token (PAT) 

在 GitHub 上获取 **Personal Access Token (PAT)** 的步骤如下：

------

### **1. 登录 GitHub 账户**

- 访问 [GitHub 官网](https://github.com) 并登录你的账户。

### **2. 进入 Token 设置页面**

- 点击右上角头像 → **Settings** → 左侧菜单栏选择 **Developer settings** → **Personal access tokens** → **Tokens (classic)**。


## PicGo配置(记得配置代理-否则会上传失败).
下载最新版-PicGo-Setup-2.4.0-beta.9.exe（直接安装即可）：
```
https://picgo-release.molunerfinn.com/2.4.0-beta.9/PicGo-Setup-2.4.0-beta.9.exe
```

picgo设置-设置代理和镜像地址-查看代理端口（7890比较口）：
```
http://127.0.0.1:7897
```

图床设置:
![图床设置](https://raw.githubusercontent.com/AylerH/ImagehostingOnlineUrl/master/image_files/picgo-github%E8%AE%BE%E7%BD%AE.png)
```
仓库名：[github用户名]/[第一步新建的仓库名称]

分支：默认master，从2020.10.01开始，github的默认分支名变更为main

设定token：第一步创建的token

指定存储路径：可填可不填，如果填写了，图片就会存储在img文件夹下
```

## 获取图片的url
打开picgo-相册-指定图片下面-左边第一个复制按钮-复制url；
```
https://raw.githubusercontent.com/AylerH/ImagehostingOnlineUrl/master/image_files/picgo-github%E8%AE%BE%E7%BD%AE.png
```
![获取方法](https://raw.githubusercontent.com/AylerH/ImagehostingOnlineUrl/master/image_files/picgo相册-url.png)