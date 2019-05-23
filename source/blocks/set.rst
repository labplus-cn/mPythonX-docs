集合
======

集合（set）是一个无序的不重复元素序列。可以使用大括号 { } 或者 set() 函数创建集合，注意：创建一个空集合必须用 set() 而不是 { }，因为 { } 是用来创建一个空字典。


set.intersection_update(set1, set2 ... etc)
-------------

**描述：**  修改当前集合，保留与参数中的集合的相同元素

.. image:: /images/blocks/set/set.png
    :scale: 90 %

set.intersection_update(set1, set2 ... etc)

    - ``set1`` - 必需，要查找相同元素的集合
    - ``set2`` - 可选，其他要查找相同元素的集合，可以多个，多个使用逗号 , 隔开


set.update(set)
-------------

**描述：**  修改当前集合，可以添加新的元素或集合到当前集合中，如果添加的元素在集合中已存在，则该元素只会出现一次，重复的会忽略

set.update(set)

    - ``set`` - 必需，可以是元素或集合


set.difference_update(set)
-------------

**描述：**  修改当前集合，移除两个集合中都存在的元素

set.difference_update(set)

    - ``set`` - 必需，可以是元素或集合

示例
^^^^^

.. image::  /images/blocks/set/example/set.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/set/set.xml>`


set.issubset(set)
-------------

**描述：**  判断当前集合是否为指定集合的子集，如果是则返回 True，否则返回 False。

.. image:: /images/blocks/set/issubset.png
    :scale: 90 %

set.issubset(set)

    - ``set`` - 必需，指定集合


set.issuperset(set)
-------------

**描述：**  判断当前集合是否为指定集合的超集，如果是则返回 True，否则返回 False。

set.issuperset(set)

    - ``set`` - 必需，指定集合


set.pop()
-------------

**描述：**  随机移除一个元素并返回之

.. image:: /images/blocks/set/pop.png
    :scale: 90 %

示例
^^^^^

.. image::  /images/blocks/set/example/setEg.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/set/setEg.xml>`
