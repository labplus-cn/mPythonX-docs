事件
======

按键、引脚、定时器、子线程等事件指令

button_[a,b].irq(handler=None, trigger=(Pin.IRQ_FALLING | Pin.IRQ_RISING), priority=1, wake=None)
-------------

**描述：**  按键中断事件

| button_[a,b].irq(handler=None, trigger=(Pin.IRQ_FALLING | Pin.IRQ_RISING), priority=1, wake=None)

    - ``trigger`` - trigger 配置可以触发中断的事件，可能的值是：Pin.IRQ_FALLING 下降沿中断；Pin.IRQ_RISING 上升沿中断；Pin.IRQ_LOW_LEVEL 低电平中断；Pin.IRQ_HIGH_LEVEL 高电平中断
    - ``handler`` - handler 是一个可选的函数，在中断触发时调用，返回一个回调对象
    - ``priority`` - 设置中断的优先级，它可以采用的值是特定于端口的，但是更高的值总是代表更高的优先级
    - ``wake`` - 选择此中断可唤醒系统的电源模式，它可以是 machine.IDLE ， machine.SLEEP 或 machine.DEEPSLEEP

.. image:: /images/blocks/event/button_irq.png
    :scale: 90 %


class machine.Timer(id, ...)
-------------

**描述：**  构造给定id的新计时器对象,Id为-1构造虚拟计时器


Timer.init(*, mode=Timer.PERIODIC, period=-1, callback=None)
-------------

**描述：**  初始化计时器

| Timer.init(*, mode=Timer.PERIODIC, period=-1, callback=None)

    - ``mode`` - Timer.ONE_SHOT：计时器运行一次，直到配置完毕通道的期限到期;Timer.PERIODIC：定时器以通道的配置频率定期运行

.. image:: /images/blocks/event/Timer_init.png
    :scale: 90 %


Timer.deinit()
-------------

**描述：**  取消定时器的初始化，停止计时器，并禁用计时器外围设备

.. image:: /images/blocks/event/Timer_deinit.png
    :scale: 90 %


Timer.value()
-------------

**描述：**  获取并返回计时器当前计数值

.. image:: /images/blocks/event/Timer_value.png
    :scale: 90 %


Pin.irq(handler=None, trigger=(Pin.IRQ_FALLING | Pin.IRQ_RISING))
-------------

**描述：**  配置在引脚的触发源处于活动状态时调用的中断处理程序

| Pin.irq(handler=None, trigger=(Pin.IRQ_FALLING | Pin.IRQ_RISING))

    - ``handler`` - 是一个可选的函数，在中断触发时调用
    - ``trigger`` - 配置可以触发中断的事件，可能的值是：Pin.IRQ_FALLING 下降沿中断；Pin.IRQ_RISING 上升沿中断；Pin.IRQ_LOW_LEVEL 低电平中断；Pin.IRQ_HIGH_LEVEL 高电平中断

.. image:: /images/blocks/event/Pin_irq.png
    :scale: 90 %


_thread.start_new_thread(function, args [, kwargs])
-------------

**描述：**  启动一个新线程并返回其标识符。线程使用参数列表args（必须是元组）执行函数。可选kwargs参数指定关键字参数的字典。 当函数返回时，线程将以静默方式退出。当函数以未处理的异常终止时，将打印堆栈跟踪，然后线程退出（但其他线程继续运行）

.. image:: /images/blocks/event/_thread.png
    :scale: 90 %
