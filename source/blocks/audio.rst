音频
======

音频指令,提供音频录音播放功能,使用P8和P9引脚作为音频解码输出

.. Attention:: 目前只实现音频播放功能

audio.player_init()
-------------

**描述：**  音频播放初始化,为音频解码开辟缓存

.. image:: /images/blocks/audio/player_init.jpg
    :scale: 90 %


audio.play(url)
-------------

**描述：**  本地或网络音频播放,目前只支持mp3格式音频

| audio.play(url)

    - ``url`` - 音频文件路径,类型为字符串,可以是本地路径地址,也可以是网络上的URL地址

.. image:: /images/blocks/audio/play.jpg
    :scale: 90 %

audio.set_volume(vol)
-------------

**描述：**  设置音频音量

| audio.set_volume(vol)

    - ``vol`` - 音量设置,范围0~100

.. image:: /images/blocks/audio/set_volume.jpg
    :scale: 90 %


audio.stop()
-------------

**描述：**  音频播放停止

.. image:: /images/blocks/audio/stop.jpg
    :scale: 90 %


audio.pause()
-------------

**描述：**  音频播放暂停


audio.resume()
-------------

**描述：**  音频播放恢复,用于暂停后的重新播放


audio.player_status()
-------------

**描述：**  用于获取系统是否处于音频播放状态,返回1,说明正处于播放中,返回0,说明播放结束,处于空闲


audio.player_deinit()
-------------

**描述：**  音频播放结束后,释放缓存

.. image:: /images/blocks/audio/player_deinit.jpg
    :scale: 90 %


示例
^^^^^

.. image::  /images/blocks/audio/example/audio.jpg
    :scale: 100 %

:download:`点击下载图形化示例</../examples/audio/audio.xml>`
