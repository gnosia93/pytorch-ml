```

def func(callback = None, callback_param = None):
    print("inner call")
    if callback is not None:
        rs = callback(callback_param)
        return rs

def callback(param):
    print("callback...", param)
    return (1, 2, 3);

rs = func(callback=callback, callback_param='param')
print(rs)


```
