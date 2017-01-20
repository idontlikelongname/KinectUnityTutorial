Kinect and Unity Tutorial
====================================
这个教程的主要目的帮助大家入门Kinect以及Unity，但是不会涉及具体的知识细节，只会给大家提供一些我平时收集到的，觉得质量还不错的教程，节省大家的时间，更有效率的入门。
***********
###Author: xiaoxiao.yang
===================================

###简介
本篇教程的内容可以分为三个部分
* 了解Kinect
* 了解Unity
* 了解Kinect在Unity中的使用

具体达到什么程度算是到达“了解”水平，我会在每个部分列出具体的问题，如果能够回答这些问题，我个人认为就算是达到了“了解”的程度。这些问题也是后续做实际的开发将会遇到的问题。

-----------

###了解Kinect
介绍Kinect的博客、网站、视频很多，在这里我推荐几个。这部分内容有些涉及具体的编程，我不建议在这部分过多的涉及编程的内容，因为在Unity中Kinect的编程与这些博客中介绍的稍微有些不同，具体的编程可以在第三部分再深入了解。这部分内容侧重对Kinect整体框架知识的理解。
* [Heresy的博客](https://kheresy.wordpress.com/kinect-for-windows-v2-cpp-index/)

    Heresy的博客主要介绍了Kinect2的C++编程，与Unity下的C#编程差别较大，但是博客的第一部分[Kinect For Windows SDK v2基本介绍](https://kheresy.wordpress.com/2014/12/29/kinect-for-windows-sdk-v2-basic/)对Kinect的介绍很详细，资料也很准确，需要重点看一下。
    [Visual Gesture Builder工具的使用](https://kheresy.wordpress.com/2015/08/22/visual-gesture-builder-tool-part-1/)也值得一看
    
* [Microsoft官方视频](http://www.k4w.cn/news/2.html)

    Kinect2发布时的官方视频，详细介绍了各种Kinect的各种特性。需要重点了解的是**[03_A Kinect2.0中文视频Hand PointGesture]** **[03_B Kinect2.0中文视频PHIZ]** **[06_A Kinect2.0中文视频Studio]**。

####注意问题的
1. Kinect SDK的如何在Windows中安装，Kinect V2对电脑系统的要求，以及推荐性能。
2. Kinect SDK能提供的基本数据有哪些？彩色图像、深度图像、骨骼关节点的空间坐标等，以及这些数据的基本参数，图像分辨率，彩色图像位数，坐标单位，关节点数量，每个关节点对应身体上的哪个部位
3. Kinect骨骼关节点坐标的坐标系信息。坐标轴方向，坐标轴原点，坐标数据单位，坐标取值范围
4. Kinect SDK总共有几种坐标系？Kinect坐标系、彩色图像坐标系、深度图像坐标系，这三个坐标系之间的数据如何转换？SDK提供的骨骼点的三维数据是在什么坐标系下值？
5. Kinect Studio的使用（重点），如何在没有Kinect V2硬件的情况下调试Kinect程序，[Kinect数据包，密码5aj9](http://pan.baidu.com/s/1cAENhW)。
6. Kinect Visual Gesture Builder的使用

-----------

###了解Unity
Unity是一个入门容易，精通难的游戏开发引擎，到目前为止我也只懂一点皮毛知识，勉强够用，做开发时遇到问题也是现查现用。网上Unity的教程太多了，五花八门，我也没有特别的推荐。但是我建议大家学习Unity的时候不要一下子走的太深，因为游戏引擎的知识点太多了，一下子学的太深，长时间不用很快就会遗忘，所以在熟悉了基本操作的基础上，对Unity的功能只需大概了解一下即可，知道哪些功能能实现什么效果，当项目有具体的需要时再仔细的学习。
* [游戏蛮牛论坛](http://www.manew.com/)

    蛮牛论坛算是目前最活跃的unity论坛，里面有大量的Unity教学视频，还有很多免费的Unity插件包。可以自己在论坛里面找到Unity的入门视频。我这里分享一个我自己的[Unity教程百度网盘](http://pan.baidu.com/s/1bpqt5uR)链接，密码a5a2。
    
* [Unity官方教程](https://unity3d.com/cn/learn)

    Unity官方教程，教程简单，容易上手，Unity的特性也介绍的很清楚，每个教程还对应有工程文件下载，值得一看。
    
* [Unity安装程序百度云盘](http://pan.baidu.com/s/1qYARHYO)

    密码wtpt，目前我正在使用的Unity版本，推荐大家安装64位，链接内包含破解文件。
    
####注意问题的
1. Unity的安装与破解
2. Unity中3D和2D的碰撞体知识，OnTriggerEnter、OnColliderEnter等函数的使用
3. 如何在Unity中显示视频、图像
4. 利用uGUI搭建基本的界面
5. 如何导入插件包Package
6. Unity中坐标系的转换

-----------

###了解Kinect在Unity中的使用
Kinect在Windows下一般通过MS Kinect SDK编程，利用Unity进行Kinect编程还需要一个Unity的插件。目前流行很多个版本的插件，但是我觉得最好的，也是我经常用的一个插件是[Kinect V2 Examples with MS-SDK](https://www.assetstore.unity3d.com/en/#!/content/18708)，作者是一个澳大利亚的工程师，专门研究人机交互。插件需要购买20$，我已经购买过了，分享给大家，，[密码93eq](http://pan.baidu.com/s/1i52sZdV)。
* [插件作者网站](https://rfilkov.com/2014/08/01/kinect-v2-with-ms-sdk/)

    网站介绍了插件的基本使用方法，以及使用插件过程中常见的一些问题。我建议通过插件内的Demo学习插件的基本使用方法。然后通过实际的项目学习具体的使用方法。
    
**TODO-待后续更新**
* [策划一个实际的游戏，并提供基本的素材，从实现游戏的过程中学习和熟练知识]
* [Unity完整项目包密码n9qb](http://pan.baidu.com/s/1nuCJYeH)
    
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    
####注意问题的
1. XXXXXXXXX



##Tips
-----------------------
###Unity调用dll时，无法detach解决方法
http://answers.unity3d.com/questions/10216/unload-a-plugin.html
http://answers.unity3d.com/questions/1127916/reloading-native-plugins.html
https://blogs.msdn.microsoft.com/jonathanswift/2006/10/03/dynamically-calling-an-unmanaged-dll-from-net-c/
http://runningdimensions.com/blog/?p=5
http://answers.unity3d.com/questions/293867/easier-way-to-handle-unloading-dlls.html

###Background Remover 
http://www.technogumbo.com/2013/09/Analysis-of-the-Kinect-For-Windows-SDK-1.8-Background-Removal-API/
RawUserDepth means that only the raw depth image values, comming from the sensor will be available, via the GetRawDepthMap for instance
BodyTexture means that GetUsersLblTex will return the white image of the tracked users
UserTexture will cause GetUsersLblTex to return the tracked users' histogram image
CutOutTexture, combined with enabled 'Compute color map', means that GetUsersLblTex will return the cut-out image of the users

