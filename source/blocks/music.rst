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


range()
-------------

**描述：**  创建一个整数列表，一般用在 for 循环中

| range(start, stop[, step])    

    - ``start`` - 计数从 start 开始。默认是从 0 开始。例如range（5）等价于range（0， 5）
    - ``stop`` - 计数到 stop 结束，但不包括 stop。例如：range（0， 5） 是[0, 1, 2, 3, 4]没有5
    - ``step`` - 步长，默认为1。例如：range（0， 5） 等价于 range(0, 5, 1)

示例
^^^^^


警笛声

.. image:: /images/blocks/music/example/pitch_in_range.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/music/pitch_in_range.xml>` 


music.play()
-------------

**描述：**  播放音乐


| music.play(music, pin=6, wait=True, loop=False)

    - ``music`` - 内置音乐，如music.PYTHON；音符，如'c1:4'；音符列表，如['r4:2', 'g', 'g', 'g', 'eb:8', 'r:2', 'f', 'f', 'f', 'd:8']
    - ``pin`` - 默认是掌控板的P6引脚
    - ``wait`` - 阻塞，如果为 True 则阻塞，反之则不
    - ``loop`` - 如果 loop 设置为 True ，则重复调整直到stop被调用或阻塞调用被中断

示例
^^^^^

.. image::  /images/blocks/music/example/play.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/music/play.xml>` 


music.set_tempo()
-------------

**描述：**  设置播放节拍


| music.set_tempo(ticks=4, bpm=120)

    - ``ticks`` - 一定数量的ticks(整数)构成单个节拍
    - ``bpm`` - 每分钟节拍数






