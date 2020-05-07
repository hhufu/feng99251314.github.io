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
{% asset_img image-20200424143440500.png%}
<!-- more -->
（2）找到对应选项
{% asset_img image-20200424143531734.png%}
（3）找到项目的目录
{% asset_img image-20200424144156379.png%}
（4）选中Copy projects into workspace
{% asset_img image-20200424144218247.png%}
（5）我们发现项目导入后是报错的
{% asset_img image-20200424144251447.png%}
（6）选中项目，单击鼠标右键
{% asset_img image-20200424144320991.png%}
（7）双击报错地方（这个子窗口是Libraries）
{% asset_img image-20200424144445919.png%}

（8）点击Environments 选择 JavaSE-1.8  点击 Apply and Close，最后点击finish

{% asset_img image-20200424144543368.png%}

（9）双击  Server Library....  选择你的eclipse配置的tomcat，最后点击finish
{% asset_img image-20200424144831109.png%}

（10）最后点击Apply and Close
{% asset_img image-20200424145037668.png%}

（11）选择input.jsp 单击右键，运行
{% asset_img image-20200424145150221.png%}

（12）最后选择自己的tomcat，finish
{% asset_img image-20200424145234970.png%}

（13）发现运行后还是错误
{% asset_img image-20200424145443157.png%}

（14）我们查看项目，发现是java文件报错
{% asset_img image-20200424145510527.png%}

（15）解决办法：（如果没有出现错误，不用理睬）

选中项目，单击鼠标右键

{% asset_img image-20200424145611025.png%}

（16）我们发现，jdk错误
{% asset_img image-20200424145652376.png%}

（17）找到这里，把13改为1.8，Apply and Close
{% asset_img image-20200424145904460.png%}

（18）运行后成功解决
{% asset_img image-20200424150101096.png%}

