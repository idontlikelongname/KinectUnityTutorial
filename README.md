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
具体到达什么程度算是到达“了解”水平，我会在每个部分列出具体的问题，如果能够回答这些问题，我个人认为就算是达到了“了解”的程度。这些问题也是后续做实际的开发将会遇到的问题。
###了解Kinect
介绍Kinect的博客、网站、视频很多，在这里我推荐几个。这部分内容有些涉及具体的编程，我不建议在这部分过多的涉及编程的内容，因为在Unity中Kinect的编程与这些博客中介绍的稍微有些不同，具体的编程可以在第三部分再深入了解。这部分内容侧重对Kinect整体框架知识的理解。
* [Heresy的博客](https://kheresy.wordpress.com/kinect-for-windows-v2-cpp-index/)
    Heresy的博客主要介绍了Kinect2的C++编程，与Unity下的C#编程差别较大，但是博客的第一部分[Kinect For Windows SDK v2基本介绍](https://kheresy.wordpress.com/2014/12/29/kinect-for-windows-sdk-v2-basic/)对Kinect的介绍很详细，资料也很准确，需要重点看一下。
    [Visual Gesture Builder工具的使用](https://kheresy.wordpress.com/2015/08/22/visual-gesture-builder-tool-part-1/)也值得一看
* [Microsoft官方视频](http://www.k4w.cn/news/2.html)
    Kinect2发布时的官方视频，详细介绍了各种Kinect的各种特性。需要重点了解的是**[03_A Kinect2.0中文视频Hand PointGesture]** **[03_B Kinect2.0中文视频PHIZ]** **[06_A Kinect2.0中文视频Studio]**。
    1.Kinect SDK的安装
    3.Kinect SDK能提供的基本数据有哪些？彩色图像、深度图像、骨骼关节点的空间坐标等，以及这些数据的基本参数，图像分辨率，彩色图像位数，坐标单位，关节点数量，每个关节点对应身体上的哪个部位
    4.Kinect骨骼关节点坐标的坐标系信息。坐标轴方向，坐标轴原点，坐标数据单位，坐标取值范围
    5.Kinect SDK总共有几种坐标系？Kinect坐标系、彩色图像坐标系、深度图像坐标系，这三个坐标系之间的数据如何转换？SDK提供的骨骼点的三维数据是在什么坐标系下值？
    6.Kinect Studio的使用（重点），如何在没有Kinect V2硬件的情况下调试Kinect程序。
    7.Kinect Visual Gesture Builder的使用
