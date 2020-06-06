---
title: eclipse导入web项目的相关配置
date: 2020-05-03 17:14:26
tags:
  - Java
  - Jsp
  - Web
---
以导入ch5为例

第一步：打开eclipse，导入项目  
（1）单击File

![01](http://qb4c7lv86.bkt.clouddn.com/201.png)

<!-- more -->
（2）找到对应选项

![02](http://qb4c7lv86.bkt.clouddn.com/202.png)
（3）找到项目的目录
![02](http://qb4c7lv86.bkt.clouddn.com/203.png)
（4）选中Copy projects into workspace
![02](http://qb4c7lv86.bkt.clouddn.com/204.png)
（5）我们发现项目导入后是报错的
![02](http://qb4c7lv86.bkt.clouddn.com/205.png)
（6）选中项目，单击鼠标右键
![02](http://qb4c7lv86.bkt.clouddn.com/206.png)
（7）双击报错地方（注意：这个子窗口是Libraries）
![02](http://qb4c7lv86.bkt.clouddn.com/207.png)

（8）点击Environments 选择 JavaSE-1.8  点击 Apply and Close，最后点击finish

![02](http://qb4c7lv86.bkt.clouddn.com/208.png)

（9）双击  Server Library....  选择你的eclipse配置的tomcat，最后点击finish
![02](http://qb4c7lv86.bkt.clouddn.com/209.png)

（10）最后点击Apply and Close
![02](http://qb4c7lv86.bkt.clouddn.com/210.png)

（11）选择input.jsp 单击右键，运行
![02](http://qb4c7lv86.bkt.clouddn.com/211.png)

（12）最后选择自己的tomcat，finish
![02](http://qb4c7lv86.bkt.clouddn.com/212.png)

（13）发现运行后还是错误
![02](http://qb4c7lv86.bkt.clouddn.com/213.png)

（14）我们查看项目，发现是java文件报错
![02](http://qb4c7lv86.bkt.clouddn.com/214.png)

（15）解决办法：（如果没有出现错误，不用理睬）

选中项目，单击鼠标右键

![02](http://qb4c7lv86.bkt.clouddn.com/215.png)

（16）我们发现，jdk错误
![02](http://qb4c7lv86.bkt.clouddn.com/216.png)

（17）找到这里，把13改为1.8，Apply and Close
![02](http://qb4c7lv86.bkt.clouddn.com/2177.png)

（18）运行后成功解决
![02](http://qb4c7lv86.bkt.clouddn.com/218.png)

 (19)  如果运行的时候，出现一下以下错误，就按照15～17步骤操作![在这里插入图片描述](http://qb4c7lv86.bkt.clouddn.com/19.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80MzM5NDg0MA==,size_16,color_FFFFFF,t_70)
如果修改不了，可以参照如下修改
找到项目的目录
![在这里插入图片描述](http://qb4c7lv86.bkt.clouddn.com/220.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80MzM5NDg0MA==,size_16,color_FFFFFF,t_70)
修改它的2个属性，确认并重启eclipse![在这里插入图片描述](http://qb4c7lv86.bkt.clouddn.com/221.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80MzM5NDg0MA==,size_16,color_FFFFFF,t_70)