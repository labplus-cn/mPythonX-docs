mPython X 使用说明
====================

软件安装
-----------

最新版本为0.6.1：

* http://static.steamaker.cn/files/mpythonx-0.6.1-win.exe (Win 7 / 8 / 10)

* http://static.steamaker.cn/files/mpythonx-0.6.1-mac.zip (Mac OS)

* http://static.steamaker.cn/files/mpythonx-0.6.1-xp.exe (Win XP)

* http://static.steamaker.cn/files/mpythonx-0.5.2-linux.tar.gz (Linux x64)

* http://static.steamaker.cn/files/mpythonx-0.5.2-arm.tar.gz (树莓派)

* http://static.steamaker.cn/files/mpythonx-0.5.2-arm64.tar.gz (虚谷号、冲锋舟)


附：掌控板的Mac驱动

https://www.silabs.com/documents/public/software/Mac_OSX_VCP_Driver.zip

Mac驱动装不上的解决方案

https://www.labplus.cn/posts/5ce21e777f719d2556d121c3


.. Hint::

  安装过程有可能被杀毒软件误报病毒，需要选择“允许程序所有操作”。


安装软件的最后一步，会自动安装CP210x的驱动，如果先前安装过则可以忽略。

.. image:: /images/mPythonX/software_2.png
    :width: 500px


更新日志
-----------

0.6.1
````````
1. 掌控板固件更新到v2.2.1；

#. 优化按键、触摸键事件语法；

#. 单次上传文件改为最大1M；

#. 增加扩展：N+小方舟、MU视觉传感器等；

#. 增加UDP消息传递；

#. 增加蓝牙iBeacon室内定位及示例。

0.6.0
````````
1. 增加一个新的BLE固件；

#. 增加BLE相关功能与示例；

#. 改写讯飞语音识别与示例。

0.5.2
````````
1. 掌控板固件更新到v2.0.2；

#. 修复讯飞语音TTS；

#. 增加百度语音及示例。

0.5.1
````````
1. 掌控板固件更新到v2.0.1；

#. 优化掌控板语音识别；

#. 界面小修改。

0.5.0
````````
1. 加入硬件选择：掌控板/AI交互实验箱/micro:bit；

#. 掌控板模式下，可烧录掌控板2.0固件(兼容1.X板)；

#. 掌控板模式下，增加磁力计(仅掌控板2.0可用)、讯飞语音识别、及一些通用传感器；

#. AI交互实验箱模式下，提供实验箱专用固件与示例；

#. micro:bit模式下，相比旧版micro:bit专用软件，增加REPL区与示例。

0.3.5
````````
1. 固件更新到1.5.1，内置增加一些中国歌曲、修复舵机bug；

#. 增加可选固件：模拟 micro:bit 连 Scratch 3（测试版）；

#. 软件启动速度有所提高；

#. 检测掌控板连接情况，自动连接、断开；

#. 控制台可以 Ctrl+V 粘贴代码；

#. 增加“天气”分类，支持心知天气；

#. 支持 DS18B20 传感器；

#. 产生真随机数（通过随机种子）。

0.3.4
````````

1. 固件更新到1.5.0，可用空间扩大至2M；

#. 新增sdcard库，支持外接sd卡；

#. urequests库支持http上传二进制文件；

#. gui库支持显示bmp图片；

#. gui库支持生成并显示二维码；

#. ap模式可设置密码；

#. neopixel新增调整亮度block；

#. mqtt新增腾讯物联网block；

#. 对部分OSError增加中英文提示。

0.3.3
````````

1. 允许刷入main.py之外的其他文件；

#. 文件系统增加选取任意*.py文件运行的功能；

#. “事件”分类增加掌控板被抛起的事件。

0.3.2
````````

1. 允许香港手机号码登录小程序。

0.3.1
````````

1. 支持MQTT、EasyIoT；

#. 调整引脚下拉框编程方式；

#. 新增库函数hcsr04.py。

0.3.0
````````

1. 增加audio、tts、radio等；

#. 增加微信小程序功能；

#. 支持Tello教育版、Yeelight；

#. Blynk库升级到最新版，支持私服；

#. 增加“串口”分类，增加、优化若干block；

#. 增加“擦除固件”、“打开板载文件”等功能。

0.2.2
````````

1. 增加内置英文字体、允许自定义英文字体；

#. 增加自定义条件触发事件；

#. 对pbm图片的支持更友好；

#. python基础语法完善：增加“集合”分类、try-except-finally语法；

#. 增加"三轴倾斜角值"、"I2C超声波值"等block；

#. 调试与文件下载增加出错提示；

#. 固件内置资源更新，增加若干表情、字体。

0.2.1
````````

1. 集成tinywebio库；

#. 增加功能：只刷代码；

#. 增加自定义代码block；

#. 增加灯带彩虹效果block，及示例；

#. 增加P～N触摸事件block。

0.2.0
````````

1. 固件更新，开机动画优化；

#. 在代码出错时，OLED能提示具体错误行数；

#. 菜单功能增加：掌控内部文件系统、示例程序、中英双语；

#. 优化文件打开方式、增加信息提示、固件自检；

#. 增加文件、字典、Bluebit等分类；

#. 优化音乐、列表、元组等分类；

#. 允许用户上传pbm图片并读取、wifi能选时区等。

0.1.2
````````

1. 增加开机动画；

#. 增加 按钮/定时器/引脚电平 触发事件；

#. 增加“元组”定义。

0.1.1
````````

1. 修正tab键导致python程序出错的bug；

#. 修正变量的None定义导致python程序出错的bug；

#. 内置官方固件、Scratch固件、允许烧录自定义固件；

#. 双击图形化编程区隐藏代码区，再双击还原；

#. 图形化增加工具栏，允许鼠标放大缩小。

0.1.0
````````

1. 修复内置固件的bug；

#. 增加“检查更新”按钮；

#. 优化中文读写；

#. 红色显示报错信息、屏蔽读取文件时的回传内容。


接入硬件
-----------

点击桌面快捷方式mPython X，打开软件主界面。

.. image:: /images/mPythonX/mPythonX_1.png


用USB线接入掌控板。正确识别后，“连接串口”处会出现COM口，如下图：

.. image:: /images/mPythonX/mPythonX_2.png



上述顺序可以颠倒，即：可以先接入掌控，再打开软件。


图形编辑区
-----------

保存
````````

“保存代码”只保存程序对应的代码，后缀为py：

.. image:: /images/mPythonX/mPythonX_3.png

点击“本机读取”，加载保存的py文件：

.. image:: /images/mPythonX/mPythonX_5.png

读取效果如图：

.. image:: /images/mPythonX/mPythonX_4.png

“保存模块”保存程序对应的代码及图形化模块，后缀为xml：

.. image:: /images/mPythonX/mPythonX_6.png

点击“本机读取”，加载保存的xml文件，读取效果如图：

.. image:: /images/mPythonX/mPythonX_7.png

模块提示
````````
鼠标停留在模块上会有提示：

.. image:: /images/mPythonX/mPythonX_8.png

帮助文档
````````
在模块上，点击鼠标右键：

.. image:: /images/mPythonX/mPythonX_9.png

点击帮助，即可跳转至帮助文档：

.. image:: /images/mPythonX/mPythonX_10.png

切换图形/代码模式
````````

点击“代码模式”/“图形模式”，即可实现对应切换：

.. image:: /images/mPythonX/mPythonX_11.png

.. image:: /images/mPythonX/mPythonX_12.png

改变图形区/代码区大小
````````

鼠标停留在圈红的灰色三角上，按住左键左右拖动即可：

.. image:: /images/mPythonX/mPythonX_13.png


代码编辑区
-----------

代码联想：

.. image:: /images/mPythonX/mPythonX_14.png


运行/刷入
-----------

运行/刷入
````````

运行/刷入两种模式皆可实现程序效果。

点击“连接串口”，按钮字样变成“断开连接”，即可开始运行/刷入：

.. image:: /images/mPythonX/mPythonX_15.png

.. Note::

  “运行”的代码脱机后即失效，“刷入”的代码脱机后再次连接电源仍有效

代码查错
````````

圈红处是反馈的信息，包括硬件信息、代码报错信息等：

.. image:: /images/mPythonX/mPythonX_16.png

比如，红字为代码报错信息：

.. image:: /images/mPythonX/mPythonX_17.png

读出上一次刷入的代码
````````

点击“从掌控读出”即可读出上一次刷入的代码。


恢复固件
-----------

点击“恢复固件”，按照提示操作：

.. image:: /images/mPythonX/mPythonX_18.png

.. Hint::

  如果恢复固件失败（或超过30秒仍然一直在恢复），请先尝试关闭杀毒软件，或者选择信任esptool。5
