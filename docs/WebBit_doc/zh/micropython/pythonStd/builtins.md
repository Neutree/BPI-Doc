`Builtin`{.interpreted-text role="mod"} \-- 内建函数
====================================================

此处描述了所有内置函数和异常。它们也可通过 `builtins` 模块获取。

Functions and types
-------------------

::: {.function}
abs()
:::

::: {.function}
all()
:::

::: {.function}
any()
:::

::: {.function}
bin()
:::

::: {.bool()}
::: {.bytearray()}
::: {.bytes()}
参见CPython文档：
[bytes](https://docs.python.org/3.5/library/functions.html#bytes)
:::
:::
:::

::: {.function}
callable()
:::

::: {.function}
chr()
:::

::: {.function}
classmethod()
:::

::: {.function}
compile()
:::

::: {.complex()}
::: {.function}
delattr(obj, name)

参数名应该是一个string，这个函数从obj给出的对象中删除命名属性.
:::
:::

::: {.dict()}
::: {.function}
dir()
:::
:::

::: {.function}
divmod()
:::

::: {.function}
enumerate()
:::

::: {.function}
eval()
:::

::: {.function}
exec()
:::

::: {.function}
filter()
:::

::: {.float()}
::: {.frozenset()}
::: {.function}
getattr()
:::
:::
:::

::: {.function}
globals()
:::

::: {.function}
hasattr()
:::

::: {.function}
hash()
:::

::: {.function}
hex()
:::

::: {.function}
id()
:::

::: {.function}
input()
:::

::: {.int()}
::: {.method}
from\_bytes(bytes, byteorder)

在MicroPython中， [byteorder]{.title-ref}
参数必须是位置的（这与CPython兼容）
:::

::: {.method}
to\_bytes(size, byteorder)

在MicroPython中， [byteorder]{.title-ref}
参数必须是位置的（这与CPython兼容）
:::
:::

::: {.function}
isinstance()
:::

::: {.function}
issubclass()
:::

::: {.function}
iter()
:::

::: {.function}
len()
:::

::: {.list()}
::: {.function}
locals()
:::
:::

::: {.function}
map()
:::

::: {.function}
max()
:::

::: {.memoryview()}
::: {.function}
min()
:::
:::

::: {.function}
next()
:::

::: {.object()}
::: {.function}
oct()
:::
:::

::: {.function}
open()
:::

::: {.function}
ord()
:::

::: {.function}
pow()
:::

::: {.function}
print()
:::

::: {.function}
property()
:::

::: {.function}
range()
:::

::: {.function}
repr()
:::

::: {.function}
reversed()
:::

::: {.function}
round()
:::

::: {.set()}
::: {.function}
setattr()
:::
:::

::: {.slice()}
slice内置函数是slice对象的类型.
:::

::: {.function}
sorted()
:::

::: {.function}
staticmethod()
:::

::: {.str()}
::: {.function}
sum()
:::
:::

::: {.function}
super()
:::

::: {.tuple()}
::: {.function}
type()
:::
:::

::: {.function}
zip()
:::

Exceptions
----------

::: {.exception}
AssertionError
:::

::: {.exception}
AttributeError
:::

::: {.exception}
Exception
:::

::: {.exception}
ImportError
:::

::: {.exception}
IndexError
:::

::: {.exception}
KeyboardInterrupt
:::

::: {.exception}
KeyError
:::

::: {.exception}
MemoryError
:::

::: {.exception}
NameError
:::

::: {.exception}
NotImplementedError
:::

::: {#OSError}
::: {.exception}
OSError

参见CPython文档： `OSError` . MicroPython不实现 `errno`
属性，而是使用标准方式访问异常参数： `exc.args[0]` .
:::
:::

::: {.exception}
RuntimeError
:::

::: {.exception}
StopIteration
:::

::: {.exception}
SyntaxError
:::

::: {.exception}
SystemExit

参见CPython文档： `SystemExit` .
:::

::: {.exception}
TypeError

参见CPython文档： `SystemExit` .
:::

::: {.exception}
ValueError
:::

::: {.exception}
ZeroDivisionError
:::
