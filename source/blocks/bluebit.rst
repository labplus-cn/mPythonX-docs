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
