bluebit 模块
======

掌控板搭载 bluebit 套件的相关图形化指令


class bluebit.SHT20(i2c=i2c)
-------------

**描述：**   温湿度模块 SHT20 控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


SHT20.temperature()
-------------

**描述：**   获取温度

**返回值：**   温度,单位摄氏度


SHT20.humidity()
-------------

**描述：**   获取湿度


class bluebit.Color(i2c=i2c)
-------------

**描述：**   颜色模块控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


Color.getRGB()
-------------

**描述：**   获取 RGB 值


Color.getHSV()
-------------

**描述：**   获取 HSV 值


class bluebit.AmbientLight(i2c=i2c)[源代码]
-------------

**描述：**   数字光线模块控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


AmbientLight.getLight()
-------------

**描述：**   获取光线值

**返回值：**   返回光线值,单位lux


class bluebit.Ultrasonic(i2c=i2c)
-------------

**描述：**   超声波模块控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


Ultrasonic.distance()
-------------

**描述：**   获取超声波测距

**返回值：**   返回测距,单位cm


class bluebit.SEGdisplay(i2c=i2c)
-------------

**描述：**   4段数码管模块 tm1650 控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


SEGdisplay.numbers(x)
-------------

**描述：**   数字显示-999~9999

**参数：**

- ``x (int)`` - 数字,范围-999~9999


SEGdisplay.Clear()
-------------

**描述：**   数码管清屏


class Matrix(i2c=i2c)
-------------

**描述：**   8x8点阵模块控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


Matrix.blink_rate(rate=None)
-------------

**描述：**   设置像素点闪烁率

**参数：**

- ``rate`` - 闪烁间隔时间,单位秒.默认None,常亮


Matrix.brightness(brightness)
-------------

**描述：**   设置像素点亮度

**参数：**

- ``brightness`` - 亮度级别,范围0~15


Matrix.fill(color)
-------------

**描述：**   填充所有

**参数：**

- ``color`` - 1亮;0灭


Matrix.bitmap(bitmap)
-------------

**描述：**   显示位图

**参数：**

- ``bitmap`` - 8x8点阵数据


Matrix.show()
-------------

**描述：**   显示生效


class bluebit.LCD1602(i2c=i2c)
-------------

**描述：**   LCD1602 模块控制类

**参数：**

- ``i2c`` - I2C 实例对象,默认 i2c=i2c


LCD1602.LEFT_TO_RIGHT
-------------

**描述：**   文本方向常量-从左到右


LCD1602.RIGHT_TO_LEFT
-------------

**描述：**   文本方向常量-从右到左


LCD1602.Init()
-------------

**描述：**   初始化函数


LCD1602.Print(str)
-------------

**描述：**   打印字符串

**参数：**

- ``str (str)`` - 显示字符串,只支持英文


LCD1602.Clear()
-------------

**描述：**   清屏


LCD1602.setCursor(col, row)
-------------

**描述：**   设置光标位置

**参数：**

- ``col (int)`` - 列,1~16
- ``row (int)`` - 行,1~2


LCD1602.Cursor(show)
-------------

**描述：**   光标显示使能

**参数：**

- ``show (bool)`` - True or False


LCD1602.Blink(blink)
-------------

**描述：**   光标闪烁使能

**参数：**

- ``blink (bool)`` - True or False


LCD1602.display(enable)
-------------

**描述：**   设置光标位置

**参数：**

- ``enable (bool)`` - True or False


LCD1602.move_left()
-------------

**描述：**   左滚动显示


LCD1602.move_right()
-------------

**描述：**   右滚动显示


LCD1602.text_direction
-------------

**描述：**   文本方向


class bluebit.MIDI(tx)
-------------

**描述：**   MIDI 模块控制类

**参数：**

- ``tx`` - 发送引脚


MIDI.volume
-------------

**描述：**   设置或返回音量


MIDI.instrument
-------------

**描述：**   设置或返回音色


MIDI.note(note, on_off)
-------------

**描述：**   播放音符

**参数：**

- ``note`` - MIDI 音符编码
- ``on_off`` - 音符播放或停止


class bluebit.MP3(tx)
-------------

**描述：**   MIDI 模块控制类

**参数：**

- ``tx`` - 发送引脚


MP3.play_song(num)
-------------

**描述：**   播放歌曲

**参数：**

- ``num (int)`` - 歌曲编号,类型为数字


MP3.play()
-------------

**描述：**   播放,用于暂停后的重新播放


MP3.playDir(dir, songNo)
-------------

**描述：**   播放指定文件夹指定歌曲

**参数：**

- ``dir (int)`` - 文件夹编号,类型数字
- ``songNo (int)`` - 歌曲编号,类型为数字


MP3.playNext()
-------------

**描述：**   播下一首


MP3.playPrev()
-------------

**描述：**   播上一首


MP3.pause()
-------------

**描述：**   暂停播放


MP3.stop()
-------------

**描述：**   停止播放


MP3.loop(songNo)
-------------

**描述：**   目录内指定序号歌曲循环播放

**参数：**

- ``songNo (int)`` - 歌曲编号,类型为数字


MP3.loopDir(dir)
-------------

**描述：**   指定目录内循环播放

**参数：**

- ``dir (int)`` - 文件夹编号,类型数字


MP3.singleLoop(onOff)
-------------

**描述：**   单曲循环开关

**参数：**

- ``onOff (int)`` - 0:不循环 1：循环


MP3.volume
-------------

**描述：**   设置或返回音量设置,范围0~30


MP3.resetDevice()
-------------

**描述：**   复位MP3


class bluebit.OLEDBit(rx, tx)
-------------

**描述：**   OLED 模块控制类

.. image:: /images/blocks/bluebit/image160.png
    :scale: 90 %

**参数：**

- ``rx, tx`` - 接收,发送引脚


OLEDBit.font_5x7
-------------

**描述：**   字体常量-5*7英文字体


OLEDBit.font_song16
-------------

**描述：**   字体常量-16*16宋体


OLEDBit.font_song24
-------------

**描述：**   字体常量-24*24宋体


OLEDBit.font_consol32
-------------

**描述：**   字体常量-32*32宋体


OLEDBit.Print(str, x, y, font)
-------------

**描述：**   显示中英文字符串,支持字体 '0' =Font5x7, '1' = 宋体16x16, '2' = 宋体24x24, '3' = Consolas32x32

.. image:: /images/blocks/bluebit/image161.png
    :scale: 90 %

**参数：**

- ``str (str)`` - 中英文字符串
- ``x y (int)`` - 显示坐标
- ``font`` - 字体类型, font_5x7 , font_song24 , font_consol32


OLEDBit.clear(x0=0, y0=0, x1=127, y1=63)
-------------

**描述：**   清除,默认全屏清除,也可以局部清除

.. image:: /images/blocks/bluebit/image162.png
    :scale: 90 %

**参数：**

- ``x0 y0 (int)`` - 抹去区域左上坐标
- ``x1 y1 (int)`` - 抹去区域右下坐标


OLEDBit.show()
-------------

**描述：**   显示生效,当使用 framebuf 类方法后使用 show() 刷新屏幕


OLEDBit.Bitmap(x, y, bitmap, w, h, c)
-------------

**描述：**   显示图案

.. image:: /images/blocks/bluebit/image163.png
    :scale: 90 %

**参数：**

- ``x y (int)`` - 起点坐标
- ``bitmap`` -  图案1bit数据
- ``w,h`` -  图案宽高
- ``c`` -  颜色,1 or 0


class bluebit.IRRecv(rx, uart_id=1)
-------------

**描述：**   红外接收模块

**参数：**

- ``rx (int)`` - 接收引脚设置
- ``uart_id`` -  串口号:1、2


IRRecv.recv()
-------------

**描述：**   接收数据

**返回值：**  返回红外值,类型整形


class bluebit.IRTrans(tx, uart_id=2)
-------------

**描述：**   红外发射模块

.. image:: /images/blocks/bluebit/image165.png
    :scale: 90 %

**参数：**

- ``tx (int)`` - 发送引脚设置
- ``uart_id`` -  串口号:1、2


IRTrans.transmit(byte)
-------------

**描述：**   发送数据

.. image:: /images/blocks/bluebit/image164.png
    :scale: 90 %

**参数：**

- ``byte (byte)`` - 发送数据,单字节
