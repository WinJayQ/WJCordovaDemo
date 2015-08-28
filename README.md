# WJCordovaDemo
  打开 platforms/ios/IOSPrj.xcodeproj 可以运行。


#                 Cordova—iOS教程

##一、Cordova说明：
   Cordova提供了一组设备相关的API，通过这组API，移动应用能够以JavaScript访问原生的设备功能，如摄像头、麦克风等。 Cordova还提供了一组统一的JavaScript类库，以及为这些类库所用的设备相关的原生后台代码。 Cordova支持如下移动操作系统：iOS, Android,ubuntu phone os, Blackberry, Windows Phone, Palm WebOS, Bada 和 Symbian。
Cordova是贡献给Apache后的开源项目，是从PhoneGap中抽出的核心代码，是驱动PhoneGap的核心引擎。你可以把他想象成类似于Webkit和Google Chrome的关系。

##二、环境配置，新建项目
###1. 如果你的terminal不能运行 npm，那先得安装 Node.js
   Node文件夹下的node-v0.12.7.pkg
   下载链接：http://nodejs.org/download/ 

###2. 在命令行terminal利用 npm安装 Cordova

     sudo npm install -g cordova
     
###3.开始建立第一个CordovaIOSPrj的应用
####3.1 创建项目

    cordova create CordovaIOSPrj com.example.CordovaIOSPrj IOSPrj  -d
  
-d 是为了在过程中能输出信息。
之后，在你运行上面这条命令的路径下，就会建立一个"CordovaIOSPrj"的目录。在CordovaIOSPrj目录下有一个 "www"的目录，将是你应用的hompage的目录。

####3.2cd到CordovaIOSPrj目录，到执行命令，为CordovaIOSPrj添加iOS的平台支持

    cordova platform add ios
   
执行成功后，在CordovaIOSPrj/platforms/下面就会多了一个ios的目录了。

####3.3 运行下面命令build项目
    cordova build
    
一堆信息过后，最后出现"BUILD SUCCEEDED"
之后，就可以，在xCode中打开该项目。选择"platforms/ios/IOSPrj.xcodeproj"文件打开。

效果图：
   ![image](https://github.com/WinJayQ/WJCordovaDemo/raw/master/wj1.png)
   

##三、添加plugin

###添加设备API:

    cordova plugin add cordova-plugin-device
  
###网络连接：

    cordova plugin add cordova-plugin-network-information

###电池：

    cordova plugin add cordova-plugin-battery-status

###加速度计：

    cordova plugin add cordova-plugin-device-motion

###地理定位：

    cordova plugin add cordova-plugin-geolocation

###相机：

    cordova plugin add cordova-plugin-camera

###媒体重播和捕获：

    cordova plugin add cordova-plugin-media-capture
    cordova plugin add cordova-plugin-media

###联系人：

    cordova plugin add cordova-plugin-contacts

###其他参考Apache Cordova Documentation


###四、加入html，CSS，JS等文件

运行效果图：
    ![image](https://github.com/WinJayQ/WJCordovaDemo/raw/master/wj2.png)


##五、常用Native API的使用

###5.1 Accelerometer(加速计传感器) 
html代码见“Cordova-iOS教程.docx”文档

###5.2 Camera(摄像头) 

html代码见“Cordova-iOS教程.docx”文档

###5.3 Device(设备信息) 

html代码见“Cordova-iOS教程.docx”文档

###5.4 Connection(网络连接状态)

html代码见“Cordova-iOS教程.docx”文档

###5.5 Geolocation(GPS地理位置服务) 

html代码见“Cordova-iOS教程.docx”文档

###5.6 File(文件系统处理 ) 

html代码见“Cordova-iOS教程.docx”文档

###5.7 Database(客户端数据库) 

html代码见“Cordova-iOS教程.docx”文档



