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
# api相关
api文档：https://picgo.github.io/PicGo-Core-Doc/zh/api/

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

# PicGo常用插件总结

## 图片处理插件

1. **picgo-plugin-compress**
   - **功能**：上传前自动压缩图片，减小文件体积
   - **优势**：节省存储空间，加快图片加载速度
   - **适用场景**：博客、文档中需要优化图片大小的场合

2. **picgo-plugin-watermark**
   - **功能**：为上传的图片添加水印
   - **优势**：保护图片版权，增加品牌标识
   - **适用场景**：需要版权保护的图片、摄影作品分享

3. **picgo-plugin-autocopy**
   - **功能**：上传完成后自动复制图片URL到剪贴板
   - **优势**：简化工作流程，提高效率
   - **适用场景**：频繁插入图片链接的写作场景

## 文件命名与管理插件

4. **picgo-plugin-rename-file**
   - **功能**：自定义上传图片的文件名规则
   - **优势**：便于管理和分类图片
   - **适用场景**：需要规范命名的团队协作环境

5. **picgo-plugin-super-prefix**
   - **功能**：为图片URL添加自定义前缀
   - **优势**：更灵活的文件组织方式
   - **适用场景**：按项目或类别组织图片的需求

6. **picgo-plugin-folder-sync**
   - **功能**：同步本地文件夹到图床
   - **优势**：批量上传和管理图片
   - **适用场景**：需要批量迁移图片的情况

## 图床扩展插件

7. **picgo-plugin-gitee**
   - **功能**：增加对码云(Gitee)图床的支持
   - **优势**：提供国内访问更快的图床选项
   - **适用场景**：面向国内用户的网站、博客

8. **picgo-plugin-s3**
   - **功能**：支持亚马逊S3及兼容S3协议的存储服务
   - **优势**：扩展更多云存储选择
   - **适用场景**：使用AWS或其他S3兼容存储的用户

9. **picgo-plugin-piclist**
   - **功能**：为PicGo增加图片列表管理功能
   - **优势**：更好地组织和查找已上传的图片
   - **适用场景**：管理大量图片资源的用户

## 编辑器集成插件

10. **picgo-plugin-vscode-migrator**
    - **功能**：支持与VS Code PicGo插件配置同步
    - **优势**：无缝集成代码编辑和图片上传工作流
    - **适用场景**：同时使用VS Code和PicGo的开发者

11. **picgo-plugin-server**
    - **功能**：为PicGo提供HTTP API服务
    - **优势**：允许其他应用程序通过API调用PicGo上传图片
    - **适用场景**：需要与其他应用集成的高级用户

## 工作流优化插件

12. **picgo-plugin-quick-capture**
    - **功能**：快速截图并上传
    - **优势**：简化截图-上传流程为一步操作
    - **适用场景**：需要频繁截图的技术文档创作

13. **picgo-plugin-web-uploader**
    - **功能**：从网页直接上传图片到PicGo
    - **优势**：扩展PicGo使用场景
    - **适用场景**：浏览网页时需要保存并分享图片

## 安装使用方法

1. 打开PicGo主界面
2. 点击"插件设置"
3. 在搜索框中输入插件名称
4. 点击"安装"按钮
5. 根据插件文档进行相应配置

通过合理搭配这些插件，可以打造一个高效、功能丰富的图片上传和管理工作流，大幅提升写作和内容创作的效率。
