# Xcalar

这个公司是一个 startup，只有三十分钟，我做了一题多一点。

# Json 和 Object 互相转换

简单题目是从一个 Object，其实就是一个 map，输出对应的 Json，因为有嵌套的部分在，我用的是 ArrayList + 递归来实现的。

接下来是从一个 Json 转换回 Object，也就是 map。这个比较有难度，首先不能简单分割字符串，因为有嵌套，所以是逐个读入进行处理。

1. 如果碰到 `{`，那么新建一个 map
2. 读入对应的 key 和 value，并添加到之前创建的 map 中
3. 如果碰到嵌套，那么递归调用返回一个 map 作为 key
4. 最后返回最终的 map。

