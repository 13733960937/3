# 元组

Python的元组与列表类似，不同之处在于**元组的元素不能修改**。元组使用小括号，列表使用方括号。

```python
>>> aTuple = ('et',77,99.9)
>>> aTuple
('et',77,99.9)
```

#### <1>访问元组

![](../Images/Snip20160815_301.png)


#### <2>修改元组

![](../Images/Snip20160815_303.png)

说明：
**python中不允许修改元组的数据，包括不能删除其中的元素。**

#### <3>count, index

index和count与字符串和列表中的用法相同

```python
>>> a = ('a', 'b', 'c', 'a', 'b')
>>> a.index('a', 1, 3) # 注意是左闭右开区间
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: tuple.index(x): x not in tuple
>>> a.index('a', 1, 4)
3
>>> a.count('b')
2
>>> a.count('d')
0
```