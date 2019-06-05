扩展板
======

掌控板扩展板的相关图形化指令


parrot.MOTOR_1
-------------

**描述：**   M1电机编号，0x01


parrot.MOTOR_2
-------------

**描述：**   M2电机编号，0x02


parrot.set_speed(motor_no, speed)
-------------

**描述：**   设置电机速度

**参数：**

- ``motor_no (int)`` - 控制电机编号，可以使用 MOTOR_1, MOTOR_2, 或者直接写入电机编号
- ``speed (int)`` - 电机速度，范围-100~100，负值代表反转

.. image:: /images/blocks/expandBoard/1.png
    :scale: 90 %


parrot.get_speed(motor_no)
-------------

**描述：**   返回电机速度

.. image:: /images/blocks/expandBoard/3.png
    :scale: 90 %

**参数：**

- ``motor_no (int)`` - 控制电机编号，可以使用 MOTOR_1, MOTOR_2, 或者直接写入电机编号


parrot.led_on(no, brightness=50)
-------------

**描述：**   打开灯。电机接口,除了可以驱动电机,还能做灯的控制

.. image:: /images/blocks/expandBoard/4.png
    :scale: 90 %

**参数：**

- ``no (int)`` - 控制电机编号，可以使用 MOTOR_1, MOTOR_2, 或者直接写入电机编号
- ``brightness (int)`` - 设置亮度,范围0~100


parrot.led_off(no)
-------------

**描述：**   关闭灯

.. image:: /images/blocks/expandBoard/5.png
    :scale: 90 %

**参数：**

- ``no (int)`` - 控制电机编号，可以使用 MOTOR_1, MOTOR_2, 或者直接写入电机编号
