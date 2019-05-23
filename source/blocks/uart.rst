串口
====


UART(双工串行通信总线) 实现标准 UART / USART 双工串行通信协议。在物理层面，它由2根线组成：RX 和 TX。 通信单元是一个字符（不要与字符串混淆），可以是8bit或9bit宽


class machine.UART(id, baudrate, bits, parity, stop, tx, rx, rts, cts, timeout)

**描述：**   构建对象

**参数：**

- ``id`` - 串口号:1、2
- ``baudrate`` - 波特率
- ``bits`` - 每个字符的位数
- ``parity`` - 奇偶校验:0-偶数,1-奇数
- ``stop`` - UART 读、写引脚
- ``tx,rx`` - 停止位数量:1、2
- ``timeout`` - 超时时间（单位：毫秒） < timeout ≤ 0x7FFF FFFF (十进制：0 < timeout ≤ 2147483647)

.. image:: /images/blocks/uart/1.png
    :scale: 90 %

.. Attention:: ``UART(id=0)`` 用于 ``REPL``; 所有引脚均可以作为串口的输入 RX，除 ``P2``、``P3`` 、``P4`` 、``P10`` 只能作为输入，其余所有的引脚理论上都可以作为输出 TX; ``GPIO 1`` 、``GPIO 3`` 用于掌控板的 USB 串口，在初始化 UART 定义 tx ，rx 引脚一般不使用，除非你要用到掌控板的 USB 接口作为串口输出


UART.init(baudrate, bits, parity, stop, tx, rx, rts, cts, timeout)

**描述：**   使用给定参数初始化UART总线


UART.deinit()

**描述：**   关闭 UART 总线

.. image:: /images/blocks/uart/9.png
    :scale: 90 %


UART.any()

**描述：**   返回一个整数，计算可以无阻塞地读取的字符数。如果没有可用字符，它将返回0，如果有字符，则返回正数。 即使有多个可读的字符，该方法也可以返回1

.. image:: /images/blocks/uart/5.png
    :scale: 90 %


UART.read([nbytes])

**描述：**   读字符。如果 nbytes 指定，则最多读取多个字节，否则读取尽可能多的数据

**返回值：**   包含读入的字节的字节对象。 None 超时时返回

.. image:: /images/blocks/uart/7.png
    :scale: 90 %


UART.readinto(buf[, nbytes])

**描述：**   将字节读入 buf 。如果 nbytes 指定，则最多读取多个字节。否则，最多读取 len(buf) 字节数

**返回值：**   读取和存储到超时 buf 或 None 超时的字节数


UART.readline()

**描述：**   读一行，以换行符结尾

**返回值：**   读取行或 None 超时的字节数

.. image:: /images/blocks/uart/6.png
    :scale: 90 %


UART.write(buf)

**描述：**   将字节缓冲区写入总线

**返回值：**   写入或 None 超时的字节数

.. image:: /images/blocks/uart/2.png
    :scale: 90 %
