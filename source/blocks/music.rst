音乐
======

音乐控制类指令

buzz.off()
-------------

**描述：**  关闭蜂鸣器

.. image:: /images/blocks/music/buzz.off.png
    :scale: 90 %


buzz.on()
-------------

**描述：**  设置蜂鸣器音调

.. image:: /images/blocks/music/buzz.on.1.png
    :scale: 90 %

.. image:: /images/blocks/music/buzz.on.2.png
    :scale: 90 %

| buzz.on(freq=500)

    - ``freq`` - 默认500Hz，0 < freq ≤ 78125


music.pitch()
-------------

**描述：**  播放一定时长的频率

.. image:: /images/blocks/music/pitch.png
    :scale: 90 %

| music.pitch(frequency, duration=-1, pin=6, wait=True)

    - ``frequency`` - 频率
    - ``duration`` - 毫秒数，如果为负，则连续播放频率，直到阻塞或者被中断，或者在后台呼叫的情况下，设置或调用新频率stop
    - ``pin`` - 默认是掌控板的P6引脚，一次只能在一个引脚上播放频率
    - ``wait`` - 阻塞，如果为 True 则阻塞，反之则不

示例
^^^^^

.. image::  /images/blocks/music/example/pitch.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/music/pitch.xml>` 

