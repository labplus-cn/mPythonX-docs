引脚
=====

引脚控制类指令

pin.read_digital()
-------------

**描述：**  读取IO引脚电平值，1代表高电平，0代表低电平

.. image:: /images/blocks/pin/read_digital.png
    :scale: 90 %

| pin = MPythonPin(pin_num,PinMode.IN)
| pin.read_digital()

    - ``pin_num`` - 掌控板引脚编号

示例
^^^^^

串口打印读取引脚值

.. image::  /images/blocks/pin/example/read_digital.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/pin/read_digital.xml>`


pin.write_digital()
-------------

**描述：**  设置IO引脚的高低电平，1为高电平,0为低电平

.. image:: /images/blocks/pin/write_digital.png
    :scale: 90 %

| pin = MPythonPin(pin_num,PinMode.OUT)
| pin.write_digital()

    - ``pin_num`` - 掌控板引脚编号

示例
^^^^^

IO引脚高低电平切换

.. image::  /images/blocks/pin/example/write_digital.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/pin/write_digital.xml>`


pin.read_analog()
-------------

**描述：**  读取IO引脚的模拟输入

.. image:: /images/blocks/pin/read_analog.png
    :scale: 90 %

| pin = MPythonPin(pin_num,PinMode.ANALOG)
| pin.read_analog()

    - ``pin_num`` - 掌控板引脚编号


pin.write_analog()
-------------

**描述：**  设置IO引脚的PWM输出

.. image:: /images/blocks/pin/write_analog.png
    :scale: 90 %

| pin = MPythonPin(pin_num,PinMode.PWM)
| pin.write_analog()

    - ``pin_num`` - 掌控板引脚编号

示例
^^^^^

.. image::  /images/blocks/pin/example/write_analog.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/pin/write_analog.xml>`
