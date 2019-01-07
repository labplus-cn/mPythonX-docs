显示
=====


oled.DispChar()
-----------

**描述：** oled屏显示文本

.. image:: /images/blocks/oled/DispChar.png
    :scale: 100 %


oled.DispChar(s, x, y)

参数：

    - ``s`` -需要显示的文本。
    - ``x`` 、``y`` -文本的左上角作为起点坐标。

示例
^^^^^


显示 hello,world！

.. image:: /images/blocks/oled/example/hello.png
    :scale: 60 %


oled.show()
----------

**描述：** 将缓存发送至oled显示。

.. image:: /images/blocks/oled/show.png
   :scale: 110 %


oled.show()


示例
^^^^^


显示 hello,world！

.. image:: /images/blocks/oled/example/hello.png
    :scale: 60 %

oled.fill()
-------------

**描述：**  点亮或者熄灭所有屏幕像素点。

.. image:: /images/blocks/oled/fill.png
    :scale: 80 %


oled.fill(c)

参数：

    - ``c`` - 为1时,像素点亮；为0时,像素点灭。
 
示例
^^^^^


1秒间隔,全屏亮灭  


.. image:: /images/blocks/oled/example/blink.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/oled/oled_blink.xml>` 


oled.invert()
-------------

**描述：**  翻转像素点,设置黑底、白底。

.. image:: /images/blocks/oled/invert.png
    :scale: 80 %

oled.invert(n)

参数：

    - ``n`` - 当n=1时,未填充像素点点亮,填充像素点灭。当n=0时,则反。默认启动是填充像素点点亮。

示例
^^^^^

.. image:: /images/blocks/oled/example/invert.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/oled/oled_invert.xml>` 


oled.pixel()
-------------

**描述：**  点亮或熄灭坐标像素点

.. image:: /images/blocks/oled/pixel.png
    :scale: 90 %

oled.pixel(x, y,c)

参数：

    - ``x`` , ``y`` - 像素点坐标
    - ``c`` - 当为1时,点亮；当为0时,熄灭

 
oled.circle()
-------------

**描述：**  绘制空心圆。

.. image:: /images/blocks/oled/circle.png
    :scale: 80 %

oled.circle(x, y, radius, c)

参数：

    - ``x`` 、 ``y`` -左上角作为起点坐标
    - ``radius`` - 圆半径大小
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭

示例
^^^^^

.. image:: /images/blocks/oled/example/circle.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/oled/oled_circle.xml>` 


oled.fill_circle()
-------------

**描述：**  绘制实心圆。

.. image:: /images/blocks/oled/fill_circle.png
    :scale: 80 %

oled.fill_circle(x, y, radius, c)

参数：

    - ``x`` 、 ``y`` -左上角作为起点坐标
    - ``radius`` - 圆半径大小
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭

示例
^^^^^

.. image:: /images/blocks/oled/example/fill_circle.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/oled/oled_fill_circle.xml>` 


oled.triangle()
-------------

**描述：**  绘制空心三角形。

.. image:: /images/blocks/oled/triangle.png
    :scale: 80 %

oled.triangle(x0, y0, x1, y1, x2, y2, c)

参数：

    - ``x0`` 、 ``y0`` -三角形上顶点坐标
    - ``x1`` 、 ``y1`` -三角形左顶点坐标
    - ``x2`` 、 ``y2`` -三角形右顶点坐标
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭

示例
^^^^^

.. image:: /images/blocks/oled/example/triangle.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/oled/oled_triangle.xml>` 


oled.fill_triangle()
-------------

**描述：**  绘制实心三角形。

.. image:: /images/blocks/oled/fill_triangle.png
    :scale: 80 %

oled.fill_triangle(x0, y0, x1, y1, x2, y2, c)

参数：

    - ``x0`` 、 ``y0`` -三角形上顶点坐标
    - ``x1`` 、 ``y1`` -三角形左顶点坐标
    - ``x2`` 、 ``y2`` -三角形右顶点坐标
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭

示例
^^^^^

.. image:: /images/blocks/oled/example/fill_triangle.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/oled/oled_fill_triangle.xml>` 


oled.hline()
-------------

**描述：**  绘制水平线

.. image:: /images/blocks/oled/hline.png
    :scale: 80 %

oled.hline(x, y, w, c)

参数：

    - ``x`` 、 ``y`` - 起点坐标
    - ``w``  - 长度
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭

示例
^^^^^

.. image:: /images/blocks/oled/example/hline.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/oled/oled_hline.xml>` 


oled.vline()
-------------

**描述：**  绘制垂直线

.. image:: /images/blocks/oled/vline.png
    :scale: 80 %

oled.vline(x, y, l, c)

参数：

    - ``x`` 、 ``y`` - 起点坐标
    - ``l``  - 长度
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭


oled.line()
-------------

**描述：**  绘制水平线

.. image:: /images/blocks/oled/line.png
    :scale: 80 %

oled.line(x1, y1, x2, y2, c)

参数：

    - ``x1`` 、 ``y1`` - 起点坐标
    - ``x2`` 、 ``y2`` - 终点坐标
    - ``c`` - 为1时,像素点亮；c 为0时,像素点灭

示例
^^^^^

.. image:: /images/blocks/oled/example/line.png
    :scale: 80 %   

:download:`点击下载图形化示例</../examples/oled/oled_line.xml>` 


UI.ProgressBar()
-------------

**描述：**  绘制进度条

.. image::  /images/blocks/oled/ProgressBar.png
    :scale: 80 %

UI.ProgressBar(x, y, width, height, progress)

参数：

    - ``x`` 、 ``y`` -左上角作为起点坐标
    - ``width`` -进度条宽度
    - ``height`` -进度条高度
    - ``progress`` -进度条百分比

示例
^^^^^

.. image::  /images/blocks/oled/example/ProgressBar.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/oled/ProgressBar.xml>` 

UI.stripBar()
-------------

**描述：**  绘制垂直或水平的柱状条

.. image:: /images/blocks/oled/stripBar.png
    :scale: 90 %

UI.stripBar(x, y, width, height, progress,dir=1,frame=1)

参数：

    - ``x`` 、 ``y`` -左上角作为起点坐标
    - ``width`` -柱状条宽度
    - ``height`` -柱状条高度
    - ``progress`` -柱状条百分比
    - ``dir`` -柱状条方向。dir=1时水平方向,dir=0时,垂直方向。
    - ``frame`` -当frame=1时,显示外框；当frame=0时,不显示外框。

 
示例
^^^^^


.. image:: /images/blocks/oled/example/light_stripBar.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/oled/light_stripBar.xml>` 