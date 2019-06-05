逻辑
====


and
-------------

**描述：**   布尔"与"


or
-------------

**描述：**   布尔"或"


not
-------------

**描述：**   布尔"非"


None
-------------

**描述：**   空


return
-------------

**描述：**   return [表达式] 语句用于退出函数，选择性地向调用方返回一个表达式。不带参数值的 return 语句返回 None


try...except...finally
-------------

**描述：**   执行 try 语句，无异常则继续执行 try 语句；发生异常则跳转至 except 语句并执行之，执行 except 语句完毕后跳回执行 try 语句的剩余部分。无论有无异常，最后必定执行 finally 语句

.. image:: /images/blocks/logic/1.png
    :scale: 90 %


type(object)
-------------

**描述：**   返回对象类型

**参数：**

- ``object`` - 对象


eval(expression[, globals[, locals]])
-------------

**描述：**   用来执行一个字符串表达式，并返回表达式的值

.. image:: /images/blocks/logic/2.png
    :scale: 90 %

**参数：**

- ``expression`` - 表达式
- ``globals`` - 变量作用域，全局命名空间，如果被提供，则必须是一个字典对象
- ``locals`` - 变量作用域，局部命名空间，如果被提供，可以是任何映射对象
