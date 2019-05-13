列表
======

列表是最常用的Python数据类型，它可以作为一个方括号内的逗号分隔值出现，如[0, 'mpython']

list.append(obj)
-------------

**描述：**  在列表末尾添加新的对象

| list.append(obj)

    - ``obj`` - 添加到列表末尾的对象

.. image:: /images/blocks/list/list_append.png
    :scale: 90 %


list.extend(seq)
-------------

**描述：**  在列表末尾一次性追加另一个序列中的多个值（用新列表扩展原来的列表）

| list.extend(seq)

    - ``seq`` - 元素列表，可以是列表、元组、集合、字典，若为字典,则仅会将键(key)作为元素依次添加至原列表的末尾

.. image:: /images/blocks/list/list_extend.png
    :scale: 90 %


list.clear()
-------------

**描述：**  清空列表，类似于 del a[:]

.. image:: /images/blocks/list/clear.png
    :scale: 90 %


list.insert(index, obj)
-------------

**描述：**  将指定对象插入列表的指定位置

| list.insert(index, obj)

    - ``index`` - 对象obj需要插入的索引位置
    - ``obj`` - 要插入列表中的对象

.. image:: /images/blocks/list/insert.png
    :scale: 90 %


list.pop([index=-1])
-------------

**描述：**  移除列表中的一个元素（默认最后一个元素），并且返回该元素的值

| list.pop([index=-1])

    - ``index`` - 可选参数，要移除列表元素的索引值，不能超过列表总长度，默认为 index=-1，删除最后一个列表值

.. image:: /images/blocks/list/pop.png
    :scale: 90 %


str.split(str="", num=string.count(str))
-------------

**描述：**  通过指定分隔符对字符串进行切片，如果参数 num 有指定值，则仅分隔 num+1 个子字符串

| str.split(str="", num=string.count(str))

    - ``str`` - 分隔符，默认为所有的空字符，包括空格、换行(\n)、制表符(\t)等
    - ``num`` - 分割次数，默认为 -1, 即分隔所有

.. image:: /images/blocks/list/split.png
    :scale: 90 %


str.join(seq)
-------------

**描述：**  将序列中的元素以指定的字符连接生成一个新的字符串

| str.join(seq)

    - ``seq`` - 要连接的元素序列

.. image:: /images/blocks/list/join.png
    :scale: 90 %

示例
^^^^^

.. image::  /images/blocks/list/example/list.png
    :scale: 100 %

:download:`点击下载图形化示例</../examples/list/list.xml>` 
