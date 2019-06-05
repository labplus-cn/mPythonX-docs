MQTT
====


MQTT是一种基于发布 - 订阅的“轻量级”消息传递协议，用于在TCP / IP协议之上使用。 提供订阅/发布模式，更为简约、轻量，易于使用，针对受限环境（带宽低、网络延迟高、网络通信不稳定），可以简单概括为物联网打造


class MQTTClient(client_id, server, port=0, user=None, password=None, keepalive=0, ssl=False, ssl_params={})
-------------

**描述：**   构建对象

**参数：**

- ``client_id`` - mqtt 客户端的唯一的 id
- ``server`` - mqtt 代理服务器的 IP 地址
- ``port`` - mqtt 的服务器访问的端口号,一般为1883,不同平台端口会有所不一样
- ``user`` - 用于获取 mqtt 鉴权的用户名
- ``password`` - 用于获取 mqtt鉴权的 password
- ``keepalive`` - 连接保存时间,当在 keepalive 间隔时间内未有订阅或发布等包,将会自动断开连接


MQTTClient.set_callback(f)
-------------

**描述：**   为收到的订阅消息设置回调

**参数：**

- ``f`` - f(topic, msg) 为回调函数,第1参数为 topic 接收到的主题,第2参数为 msg 为该主题消息


MQTTClient.set_last_will(topic, msg, retain=False, qos=0)
-------------

**描述：**   设置 MQTT “last will” 消息。应该在 connect() 之前调用


MQTTClient.connect(clean_session=True)
-------------

**描述：**   连接到服务器。如果此连接使用存储在服务器上的持久会话，则返回 True（如果使用 clean_session = True 参数，则返回 False（默认值））


MQTTClient.disconnect()
-------------

**描述：**   断开与服务器的连接，释放资源


MQTTClient.ping()
-------------

**描述：**   Ping 服务器（响应由 wait_msg（）自动处理）


MQTTClient.publish(topic, msg, retain=False, qos=0)
-------------

**描述：**   发布消息


MQTTClient.subscribe(topic, qos=0)
-------------

**描述：**   订阅主题


MQTTClient.wait_msg()
-------------

**描述：**   等待服务器消息。订阅消息将通过 set_callback（）传递给回调集，任何其他消息都将在内部处理


MQTTClient.check_msg()
-------------

**描述：**   检查服务器是否有待处理的消息。如果是，则以与 wait_msg（）相同的方式处理，如果不是，则立即返回




示例
^^^^^

.. image::  /images/blocks/mqtt/example/mqtt.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/mqtt/mqtt.xml>`
