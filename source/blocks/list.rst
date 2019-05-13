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
