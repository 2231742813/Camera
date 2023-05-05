# Camera

ADB连接手机并调用相机拍照

手机和电脑同时连接到同一个wifi上

1、使用数据线使手机与电脑相连接

adb devices

查看连接到电脑的手机


2、开启远程adb

#开启远端adb,这一步需要手机通过USB连接到电脑

adb tcpip 5566

#结果如下：restarting in TCP mode port: 5555

3、然后断开USB

adb connect 192.168.0.113:5566

#其中192.168.0.113是手机的局域网IP地址

adb devices

#确认可以看到设备信息

原文链接：https://blog.csdn.net/qq_38316655/article/details/109190703
