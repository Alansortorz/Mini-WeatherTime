# 桌面时钟天气终端

![image-20210610140014925](https://user-images.githubusercontent.com/48275625/146625548-367bf0b5-3f76-4791-be01-af3c1b1b5f2e.png)


## 这是啥？

​	   作为入门ESP32的一个小项目——桌面时钟天气，硬件部分没有做最小系统，而是采用了一块ESP8266的模块加一块迷你的OLED屏幕，主要做了一个电源和连接线的板，采用叠层式的设计，非常简单。

![image-20210610142852863](https://user-images.githubusercontent.com/48275625/146625553-d98d2c5b-e69a-4b36-b880-c32dc0aa08e6.png)


软件部分使用的太极创客开源的天气时钟项目框架，我在其中做了一些调整和改进，当然主要还是学习别人的框架。

## 什么原理呢？

​	   可以理解为ESP8266是ESP32的低端版，或者说是旧版，也就是ESP32的性能更好。ESP8266是乐鑫公司推出的一款WiFi芯片，内置WiFi和蓝牙功能，使用非常方便，使用C++编程，或者可以使用Micro Python，集成度非常高，内置电源、滤波、功放、天线等模块，因此非常适合开发一些物联网产品，官方也提供相当多的中文资料。

​	   在软件实现上采用太极创客的一个天气时钟开源框架，太极创客的教程对于小白来说可真是太棒了，推爆好吧。项目链接在这：https://gitee.com/taijichuangke/bilibili_weather_clock_color

​		软件开发用的VSCode，原因是ArduinoIDE编译速度太慢了，而且我还没找到解决办法，于是就在VSCode上下载了插件来解决这个问题，配置教程可以参考B站这个：https://www.bilibili.com/video/BV1kf4y117Pf?from=search&seid=7192360916019599561

​		当然也可以看我的博客：
https://www.cnblogs.com/ningmeng484/p/14853925.html

​		WiFi联网用的乐鑫官方的Esp-Touch的Smart Config技术，通过一个APP联网来向周围设备发送WiFi密码数据，这项技术挺有意思的，相比于直连、Web配网来说操作上相对简单，也有一种类似Smart Config的技术，通过微信扫码进入一个微信小程序，然后通过向周围设备组播WiFi密码的方式联网。
相关演示参考BiliBili视频：https://www.bilibili.com/video/BV1Vv411p7p7/





