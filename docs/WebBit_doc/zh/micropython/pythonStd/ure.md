`ure`{.interpreted-text role="mod"} \-- 正则表达式
==================================================

::: {.module synopsis="正则表达式"}
ure
:::

这个模块实现了相应 `CPython`{.interpreted-text role="term"}
模块的一个子集，如下所述。有关更多信息，请参阅原始CPython文档:
[re](https://docs.python.org/3.5/library/re.html#module-re)

This module implements regular expression operations. Regular expression
syntax supported is a subset of CPython `re` module (and actually is a
subset of POSIX extended regular expressions).

Supported operators are:

`'.'`

:   Match any character.

`'[]'`

:   Match set of characters. Individual characters and ranges are
    supported.

`'^'`

`'$'`

`'?'`

`'*'`

`'+'`

`'??'`

`'*?'`

`'+?'`

`'()'`

:   Grouping. Each group is capturing (a substring it captures can be
    accessed with [match.group()]{.title-ref} method).

Counted repetitions (`{m,n}`), more advanced assertions, named groups,
etc. are not supported.

Functions
---------

::: {.function}
compile(regex\_str)

Compile regular expression, return [regex \<regex\>]{.title-ref} object.
:::

::: {.function}
match(regex\_str, string)

Compile *regex\_str* and match against *string*. Match always happens
from starting position in a string.
:::

::: {.function}
search(regex\_str, string)

Compile *regex\_str* and search it in a *string*. Unlike
[match]{.title-ref}, this will search string for first position which
matches regex (which still may be 0 if regex is anchored).
:::

::: {.data}
DEBUG

Flag value, display debug information about compiled expression.
:::

Regex objects {#regex}
-------------

Compiled regular expression. Instances of this class are created using
[ure.compile()]{.title-ref}.

::: {.method}
regex.match(string) regex.search(string)

Similar to the module-level functions `match`{.interpreted-text
role="meth"} and `search`{.interpreted-text role="meth"}. Using methods
is (much) more efficient if the same regex is applied to multiple
strings.
:::

::: {.method}
regex.split(string, max\_split=-1)

Split a *string* using regex. If *max\_split* is given, it specifies
maximum number of splits to perform. Returns list of strings (there may
be up to *max\_split+1* elements if it\'s specified).
:::

Match objects
-------------

Match objects as returned by [match()]{.title-ref} and
[search()]{.title-ref} methods.

::: {.method}
match.group(\[index\])

Return matching (sub)string. *index* is 0 for entire match, 1 and above
for each capturing group. Only numeric groups are supported.
:::
