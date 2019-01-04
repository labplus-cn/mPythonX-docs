
UI.stripBar()
-------------

**描述：**  绘制垂直或水平的柱状条

.. image:: /images/blocks/oled/stripBar.png
    :scale: 90 %

**Python解析**


.. method:: UI.stripBar(x, y, width, height, progress,dir=1,frame=1)

参数：

    - ``x`` 、 ``y`` -左上角作为起点坐标
    - ``width`` -柱状条宽度
    - ``height`` -柱状条高度
    - ``progress`` -柱状条百分比
    - ``dir`` -柱状条方向。dir=1时水平方向,dir=0时,垂直方向。
    - ``frame`` -当frame=1时,显示外框；当frame=0时,不显示外框。

 
**示例**


.. image:: /images/blocks/oled/example/light_stripBar.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/oled/light_stripBar.xml>` 