串口
====


UART(双工串行通信总线) 实现标准 UART / USART 双工串行通信协议。在物理层面，它由2根线组成：RX 和 TX。 通信单元是一个字符（不要与字符串混淆），可以是8bit或9bit宽


class machine.UART(id, baudrate, bits, parity, stop, tx, rx, rts, cts, timeout)
-------------

**描述：**   构建对象

**参数：**

- ``id`` - 串口号:1、2
- ``baudrate`` - 波特率
- ``bits`` - 每个字符的位数
- ``parity`` - 奇偶校验:0-偶数,1-奇数
- ``stop`` - UART 读、写引脚
- ``tx,rx`` - 停止位数量:1、2
- ``timeout`` - 超时时间（单位：毫秒） < timeout ≤ 0x7FFF FFFF (十进制：0 < timeout ≤ 2147483647)


.. Attention::- ``UART(id=0)`` - 用于 REPL
- 所有引脚均可以作为串口的输入RX，除 P2、P3 、P4 、P10 只能作为输入，其余所有的引脚理论上都可以作为输出TX
- GPIO 1 、GPIO 3 用于掌控板的USB串口，在初始化UART定义 tx ，rx 引脚一般不使用，除非你要用到掌控板的USB接口作为串口输出
