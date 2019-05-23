
wifi
=====

提供便捷的 wifi 连接网络方式或热点 wifi 功能

.. method:: wifi.connectWiFi()

**描述：** 连接 wifi 网络,连接掌控板开启的热点则无需密码

.. image:: /images/blocks/wifi/connectWiFi.png
    :scale: 90 %

**参数：**

    - ``ssid`` - WiFi网络名称
    - ``password`` - WiFi密码


.. method:: wifi.sta.ifconfig()[n]

**描述：** wifi 连接成功后,获取wifi配置信息，含 IP、netmask、getway、DNS，n为0、1、2、3

.. image:: /images/blocks/wifi/sta.ifconfig.png
    :scale: 100 %



示例
^^^^^

.. image:: /images/blocks/wifi/example/ifconfig.png
    :scale: 80 %

:download:`点击下载图形化示例</../examples/wifi/wifi_ifconfig.xml>`


.. method:: wifi.disconnectWiFi()

**描述：** 断开wifi网络连接

.. image:: /images/blocks/wifi/disconnectWiFi.png
    :scale: 100 %


.. method:: wifi.enable_APWiFi(essid,channel)

**描述：** 开启无线AP功能,用于掌控板之间的相互通信

.. image:: /images/blocks/wifi/enable_APWiFi.png
    :scale: 90 %

**参数：**

    - ``essid`` - 创建WiFi网络名称
    - ``channel`` -设置wifi使用信道,channel 1~13


.. method:: wifi.disable_APWiFi()

**描述：** 关闭无线AP

.. image:: /images/blocks/wifi/disable_APWiFi.png
    :scale: 100 %


.. method:: ntptime.settime(timezone, server)

**描述：** 将掌控板的时间与网络时间同步

.. image:: /images/blocks/wifi/ntptime.settime.png
    :scale: 100 %

**参数：**

    - ``timezone`` - 时区时间差,默认为东八区,补偿8小时
    - ``server`` - 可自行指定授时服务器,server为字符串类型,默认授时服务器为"ntp.ntsc.ac.cn"


.. method:: appserver.start()

**描述：** TinyWebIO服务后台运行，该服务为App Inventor应用提供远程控制接口的掌控板工具包

.. image:: /images/blocks/wifi/TinyWebIO.png
    :scale: 80 %


.. method:: appserver.start_foreground()

**描述：** TinyWebIO服务前台运行
