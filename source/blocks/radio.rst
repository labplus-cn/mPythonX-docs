无线广播
====

radio 模块提供无线广播功能,支持13 Channel,在相同的 Channel 内能接收到成员发出的广播消息,适合10米范围内的多板组网的通讯


radio.on()
-------------

**描述：**   开启无线功能

.. image::  /images/blocks/radio/1.png
    :scale: 90 %


radio.off()
-------------

**描述：**   关闭无线功能


radio.config(channel)
-------------

**描述：**   配置无线参数

.. image::  /images/blocks/radio/2.png
    :scale: 90 %

**参数：**

- ``channel (int)`` - 无线通道,范围1~13


radio.receive()
-------------

**描述：**   接收无线广播消息,消息以字符串形式返回。最大可接收250字节数据。如果没有接收到消息,则返回 ``None`` 。当 receive 内参数为 ``True`` ,即 receive(True) ,返回(msg,mac)的二元组。默认缺省 receive(False) ,即只返回msg

.. image::  /images/blocks/radio/4.png
    :scale: 90 %

radio.receive_bytes()
-------------

**描述：**   接收无线广播消息,消息以字节形式返回。其他同 radio.receive() 相同


radio.send()
-------------

**描述：**   发送无线广播消息,发送数据类型为字符串。当发送成功后返回 ``True``,否则返回``False``

.. image::  /images/blocks/radio/3.png
    :scale: 90 %


radio.send_bytes()
-------------

**描述：**   发送无线广播消息,发送数据类型为字节。当发送成功后返回 ``True``,否则返回``False``
