### note1
```
>>> s = [3, 4, 5]
>>> >>> s.extend([s.append(9), s.append(10)])
>>> s
[3, 4, 5, 9, 10, None, None]
```

这是因为 s.append(9) 和 s.append(10) 会在 s 后面添加两个数字，并且这两个方法没有返回值，因此 s.append(9) = None。相当于 s.extend[None, None]。
