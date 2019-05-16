bluebit 模块
======

掌控板搭载 bluebit 套件的相关图形化指令


class bluebit.SHT20(i2c=<sphinx.ext.autodoc.importer._MockObject object>)
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


class bluebit.Color(i2c=<sphinx.ext.autodoc.importer._MockObject object>)
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
