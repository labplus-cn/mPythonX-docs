Yeelight 智能灯
======


yeelight.discover_bulbs(timeout=2)
-------------

**描述：**   发现所有局域网内的Yeelight灯泡

**返回值：** 字典列表，包含网络中每个灯泡的IP，端口和功能

**参数：**

- ``timeout (int)`` - 等待回复需要多少秒。发现将总是要花这么长的时间， 因为它不知道当所有的灯泡都响应完毕时


class yeelight.Bulb(ip, port=55443, effect='smooth', duration=300, auto_on=False)
-------------

**描述：**   YeeLight的控制类

**参数：**

- ``ip (str)`` - 灯泡的IP
- ``port (int)`` - 连接灯泡的端口号，默认55443
- ``effect (str)`` - 效果类型."smooth" or "sudden"
- ``duration (int)`` - 效果的持续时间，以毫秒为单位.最小值为30.突然效果会忽略此值
- ``auto_on (bool)`` - 是否 ensure_on() 在每次操作之前调用以自动打开灯泡，如果它已关闭。这会在每条消息之前更新灯泡的属性， 每个命令会花费一个额外的消息。 如果您担心速率限制，请将其关闭并自行检查。get_properties() 或运行 ensure_on()
