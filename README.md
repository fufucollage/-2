# 身份证识别app

#### 介绍
本课题为基于Android平台的身份证识别应用程序开发。其目的是掌握Android开发技术和调用图像处理接口，实现一个功能完善、界面友好、操作简便的身份证识别应用程序。

在整个项目的设计中要实现的任务有：调用阿里云OCR接口完成识别、调用相机、获取内部存储图片、数据提取、数据库操作、识别相关界面编写、我的页面编写、首页页面编写以及界面优化等。
项目细节可参考博客：https://blog.csdn.net/m0_59310933/article/details/136403349

#### 软件架构
软件架构说明：项目采用MVC架构设计，将应用程序分为三个模块：视图（View）、控制器（Controller）和模型（Model）。其中，视图模块负责用户界面设计和与用户的交互；控制器模块负责控制应用程序的流程和业务逻辑；模型模块负责实现算法和业务数据处理。

开发环境：JDK11 
开发语言：Java 
开发工具：Android Studio 
目标 API 版本：31 

代码结构如图：​

​​![代码结构图](app/src/main/res/drawable/res_pic/%E4%BB%A3%E7%A0%81%E7%BB%93%E6%9E%84%E5%9B%BE.png)
![布局代码结构图](app/src/main/res/drawable/res_pic/%E5%B8%83%E5%B1%80%E4%BB%A3%E7%A0%81%E7%BB%93%E6%9E%84%E5%9B%BE.png)



#### 成果展示
首页：
![首页](app/src/main/res/drawable/res_pic/%E9%A6%96%E9%A1%B5.jpg)

识别页面：
![识别页面](app/src/main/res/drawable/res_pic/%E8%AF%86%E5%88%AB%E9%A1%B5%E9%9D%A2.jpg)

识别结果：
![识别结果](app/src/main/res/drawable/res_pic/%E6%9F%A5%E7%9C%8B%E7%BB%93%E6%9E%9C.jpg)

查询结果：
![查询结果](app/src/main/res/drawable/res_pic/%E6%9F%A5%E8%AF%A2%E7%BB%93%E6%9E%9C.jpg)

我的页面：
![我的页面](app/src/main/res/drawable/res_pic/%E6%88%91%E7%9A%84%E9%A1%B5%E9%9D%A2.jpg)

#### 安装教程

1.  软件安装可参考博客：https://blog.csdn.net/m0_59310933/article/details/136421146

#### 使用说明

1.  ​首先我们需要登录阿里云找到我们需要的accessKeyId和accessKeySecret，可以在阿里云个人主页中进行获取。

2.  访问网址https://common-buy.aliyun.com/?spm=api-workbench.api_explorer.0.0.6f05246fbVzBu7&commodityCode=ocr_personalcard_public_cn，开通证件照识别服务，如图所示，每月有200次免费次数可用，可按需购买次数。
![输入图片说明](app/src/main/res/drawable/res_pic/image.png)
3.  将accessKeyId和accessKeySecret复制到app/src/main/java/top/olws/idcarddetect/Client/Client.java这个文件中对应位置即可。如下图所示：
![输入图片说明](app/src/main/res/drawable/res_pic/demo.png)

4.    准备就绪后打开手机开发者模式，将USB调试这个设置为允许。之后使用数据线连接手机和电脑，在AndroidStudio中启动按钮左边显示为你的手机连接成功后，启动项目既可把该应用下载到你的手机上。

ps:本项目页面中的功能有的由于时间问题暂未实现，待后续时间充裕将会完善。
#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request
