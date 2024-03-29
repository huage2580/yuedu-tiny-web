---
title: "三目阅读watch 应用 使用教程"
date: 2021-09-01T14:56:15+08:00
draft: false
---


# 三目阅读watch 应用 使用教程

## 简介

三目阅读watch是在apple watch手表上独立使用的应用，在手表上阅读和听有声书。通过缓存WebDAV网盘的文件，实现离线阅读。  

问题反馈和交流群：558016293  

这里是视频教程[https://www.bilibili.com/video/BV16L4y1B7ed/](https://www.bilibili.com/video/BV16L4y1B7ed/)  

最近有朋友反馈ios15的蜂窝数据权限bug，会导致app没有网络，请参考第一篇文章。

## 准备资源

### 文本资源  
需要先准备你的txt文件，然后使用章节切割软件，按章节切割成独立文件；

[章节切割软件下载和教程](/post/txt%E6%96%87%E4%BB%B6%E7%AB%A0%E8%8A%82%E5%88%87%E5%89%B2%E8%BD%AF%E4%BB%B6%E6%95%99%E7%A8%8B/)  
切割完成得到一个.zip文件。zip内容，一个文件夹，包含所有章节文件。

```
 xxx.zip
  |---凡人修仙传
       |---000001-第一章xxx.txt
       |---000002-第二章xxx.txt
       |---000003-第三章xxx.txt
```

### 有声资源  
准备你的mp3或者m4a文件，统一放入到一个文件夹内。然后压缩为zip文件。zip文件内部结构如下
```
 xxx.zip
  |---这里是书名
       |---1文件名.mp3
       |---2文件名.mp3
       |---3文件名.mp3
```
> 请注意,windows的压缩软件可能会导致中文名乱码，使用 7zip 软件进行压缩。

### 7zip教程（用软件切割的不用使用7zip，自动生成压缩文件）    
先下载安装软件
链接：https://pan.baidu.com/s/1sCwuXrUKHgA38TuZK8Qqvg 
提取码：uglc  

选中你的资源文件夹，右键菜单选择7zip，添加到压缩包，参数填入`cu=on`
![QQ截图20210831214639.png](http://inews.gtimg.com/newsapp_ls/0/13940602260/0)

### 单个mp3文件

如果你不想压缩，而是直接使用mp3文件，可以直接上传到网盘，在缓存的时候选择mp3文件直接下载,下载完成会在music文件夹内。

## 准备WebDAV  
推荐使用坚果云，应用也是默认使用坚果云的服务地址，先注册一个坚果云账号，然后开启webDAV。  
![QQ图片20210831215219.png](http://inews.gtimg.com/newsapp_ls/0/13940602569/0)  

按以上操作，添加应用，得到`服务器地址`,`账号`,`应用密码`  
## 资源上传&缓存  
先把 【zip压缩文件】上传到坚果云，然后到应用内进行缓存。  
#### 设置webDAV账号  
打开应用，下滑到功能设置选项，点击出现设置页，再点击最上面的设置webDAV账号  
![webdav设置.jpg](http://inews.gtimg.com/newsapp_ls/0/13940602810/0)


如上输入你的账号密码（密码是坚果云随机生成的密码，不是你的登录密码），地址默认就是坚果云的，可以不用改。在输入的时候，可以随意输入空格（方便在手表上输入一些分词和符号），保存后会自动去掉所有空格。  

测试连接成功如上，如果提示错误请检查账号密码。如果提示系统异常，参考第一篇文章《ios15导致的网络问题》 

#### 缓存资源文件  

回到首页，选择`webdav云`选项，进入文件浏览界面。点击文件夹进入下一级，点击文件选中。  
选择你的zip资源文件后，会出现下载按钮，点击下载，开始缓存，当下载解压完成会到提示解压成功页面。

### 开始浏览书籍  

#### 文本书源   
![文本资源.jpg](http://inews.gtimg.com/newsapp_ls/0/13940603060/0)   

点按阅读界面弹出菜单，切换目录和设置样式


#### 有声书源  
![{38AA97D9-A4E7-36BD-9736-A8F21B82A203}.png](http://inews.gtimg.com/newsapp_ls/0/13940603398/0)

播放界面进度条可调节，点按进度左侧回退，右侧跳进。在获取焦点后可以通过旋钮更细致的调整进度，调节进度会暂停播放，调节后手动重新播放。

### 删除缓存文件  
书架页面直接侧滑，出现删除按钮，目前只能整个书源（文件夹）删除。