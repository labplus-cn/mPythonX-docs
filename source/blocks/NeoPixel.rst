NeoPixel
======

外部RGB灯带控制类指令

class NeoPixel(pin, n, bpp=3, timing=0)
-------------

**描述：**  构建对象

.. image::  /images/blocks/NeoPixel/class.png
    :scale: 80 %

参数：

    - ``pin`` - 输出引脚
    - ``n`` - LED灯的个数
    - ``bpp`` - bpp=3，默认为3元组RGB；bpp=4，对于具有3种以上颜色的LED，例如RGBW像素或RGBY像素,采用4元组RGBY或RGBY像素
    - ``timing`` - 默认等于0,为400KHz速率；等于1，为800KHz速率


NeoPixel.write() 
-------------

**描述：**  把数据写入RGB灯珠中


NeoPixel.fill( (r, g, b) )
-------------

**描述：**  填充所有灯珠颜色及亮度， r、g、b 为颜色亮度值，范围值为0~255


示例
^^^^^

.. image::  /images/blocks/NeoPixel/example/NeoPixel.png
    :scale: 80 %

:download:`点击下载图形化示例</../examples/NeoPixel/NeoPixel.xml>` 