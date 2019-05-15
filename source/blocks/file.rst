文件
======

文件操作


open(file, mode='r')
-------------

**描述：**  打开一个文件，并返回文件对象

open(file, mode='r')

    - ``file`` - 必需，文件路径（相对或者绝对路径）
    - ``mode`` - 可选，文件打开模式，常用选项：t，文本模式 (默认)；b，二进制模式；r，以只读方式打开文件；rb，以二进制格式打开一个文件用于只读；w，打开一个文件只用于写入；wb，以二进制格式打开一个文件只用于写入


file.close()
-------------

**描述：**  关闭文件。关闭后文件不能再进行读写操作


file.read([size])
-------------

**描述：**  从文件读取指定的字节数，如果未给定或为负则读取所有

file.read([size])

    - ``size`` - 从文件中读取的字节数


file.write(str)
-------------

**描述：**  向文件中写入指定字符串。在文件关闭前或缓冲区刷新前，字符串内容存储在缓冲区中，这时你在文件中是看不到写入的内容的。如果文件打开模式带 b，那写入文件内容时，str (参数)要用 encode 方法转为 bytes 形式，否则报错：TypeError: a bytes-like object is required, not 'str'

**返回值：** 返回的是写入的字符长度

file.write(str)

    - ``str`` - 要写入文件的字符串


示例
^^^^^

.. image::  /images/blocks/file/example/file.png
    :scale: 90 %

:download:`点击下载图形化示例</../examples/file/file.xml>`
