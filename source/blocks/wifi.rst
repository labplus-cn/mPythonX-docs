
wifi
=====

提供便捷的wifi连接网络方式或热点wifi功能

wifi.connectWiFi()
-------------

**描述：** 连接wifi网络,连接掌控板开启的热点则无需密码

.. image:: /images/blocks/wifi/connectWiFi.png
    :scale: 90 %

wifi.connectWiFi(ssid, password)

参数：

    - ``ssid`` - WiFi网络名称
    - ``password`` - WiFi密码


wifi.sta.ifconfig()
-------------

**描述：** wifi连接成功后,获取wifi配置信息。含IP、netmask、getway、DNS

.. image:: /images/blocks/wifi/sta.ifconfig.png
    :scale: 100 %

wifi.sta.ifconfig()[n]  

4元组,n为0、1、2、3

示例
^^^^^

.. image:: /images/blocks/wifi/example/ifconfig.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/wifi/wifi_ifconfig.xml>` 

wifi.disconnectWiFi()
-------------

**描述：** 断开wifi网络连接

.. image:: /images/blocks/wifi/disconnectWiFi.png
    :scale: 100 %

wifi.disconnectWiFi()


wifi.enable_APWiFi()
-------------------

**描述：** 开启无线AP功能,用于掌控板之间的相互通信

.. image:: /images/blocks/wifi/enable_APWiFi.png
    :scale: 90 %

wifi.enable_APWiFi(essid,channel)

    - ``essid`` - 创建WiFi网络名称
    - ``channel`` -设置wifi使用信道,channel 1~13


wifi.disable_APWiFi()
-------------------

**描述：** 关闭无线AP

.. image:: /images/blocks/wifi/disable_APWiFi.png
    :scale: 100 %

wifi.disable_APWiFi()

ntptime.settime()
-------------------

**描述：** 将掌控板的时间与网络时间同步

.. image:: /images/blocks/wifi/ntptime.settime.png
    :scale: 100 %
    
ntptime.settime()


appserver.start()
-------------------

**描述：** TinyWebIO服务后台运行，该服务为App Inventor应用提供远程控制接口的掌控板工具包

.. image:: /images/blocks/wifi/TinyWebIO.png
    :scale: 100 %


appserver.start_foreground()
-------------------

**描述：** TinyWebIO服务前台运行
