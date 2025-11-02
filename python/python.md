# python

## 字面量

![image-20250717104001082](/home/wybie/.config/Typora/typora-user-images/image-20250717104001082.png)

- 注释 

`#  `单行	`“”“ ”“”`多行

- 数据类型

  <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717104423649.png" alt="image-20250717104423649" style="zoom:50%;" />

### 数据转换

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717104544355.png" alt="image-20250717104544355" style="zoom:50%;" />

	万物都可以转字符串

### 关键字

![image-20250717104934788](/home/wybie/.config/Typora/typora-user-images/image-20250717104934788.png)

### 运算符

![image-20250717105119775](/home/wybie/.config/Typora/typora-user-images/image-20250717105119775.png)

案例：

`for 变量名 in (x,x)`表示一个变量的范围

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717105411422.png" alt="image-20250717105411422" style="zoom:50%;" />

变量的声明和输入：

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717105820148.png" alt="image-20250717105820148" style="zoom:50%;" />

判断语句：

```
if xx :
elif xx :
else :
```

- 数据容器：容纳多个变量,可嵌套即元素可为数组类

![image-20250717110136272](/home/wybie/.config/Typora/typora-user-images/image-20250717110136272.png)

1. 列表(list)：`namelist = ['a','b']`

   方法：

   ![image-20250717111635795](/home/wybie/.config/Typora/typora-user-images/image-20250717111635795.png)

   查找：`列表名.变量名(x)`

   <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717112046017.png" alt="image-20250717112046017" style="zoom:50%;" />

   插入：`列表名.insert(x)`

   <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717112143046.png" alt="image-20250717112143046" style="zoom:50%;" />

   追加：`列表名.append(x)` / `列表名.extend(追加列表名)`

   <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717112218089.png" alt="image-20250717112218089" style="zoom:50%;" />

   删除：`列表名.remove(x)`

   <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717112757332.png" alt="image-20250717112757332" style="zoom:50%;" />

   ->取出方法：`变量名 = 列表名.pop(x)`

   清空列表：`列表名.clear()`

   <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717112955447.png" alt="image-20250717112955447" style="zoom:50%;" />

   统计数量：`列表名.count(x)`  / `列表名.len(列表名)`

   <img src="/home/wybie/.config/Typora/typora-user-images/image-20250717113149238.png" alt="image-20250717113149238" style="zoom:50%;" />

   ![image-20250717113413400](/home/wybie/.config/Typora/typora-user-images/image-20250717113413400.png)

## 元组(tuple)：

![image-20250717113914605](/home/wybie/.config/Typora/typora-user-images/image-20250717113914605.png)

![image-20250717114147269](/home/wybie/.config/Typora/typora-user-images/image-20250717114147269.png)

->大括号的意思为传递表达式

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717114621461.png" alt="image-20250717114621461" style="zoom:50%;" />

->为什么会有“两个中括号”？
	Python 里的索引是「一层一层往里钻」的

![image-20250717143239778](/home/wybie/.config/Typora/typora-user-images/image-20250717143239778.png)

### **字符串(str)：**

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717143459904.png" alt="image-20250717143459904" style="zoom:50%;" />

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717143549822.png" alt="image-20250717143549822" style="zoom:50%;" />

替换：`字符串.replace(字符串1,字符串2)`

分割：指定分隔符字符串，存入列表 `列表名 = 字符串.split(分隔符字符串)`

规整：

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717144040672.png" alt="image-20250717144040672" style="zoom: 33%;" />

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717144154241.png" alt="image-20250717144154241" style="zoom:50%;" />

### **集合(set)：**

一个无序的不重复元素序列。集合中的元素不会重复，并且可以进行交集、并集、差集等常见的集合操作。可以使用大括号 **{ }** 创建集合，元素之间用逗号 **,** 分隔， 或者也可以使用 **set()** 函数创建集合。

![image-20250717144503668](/home/wybie/.config/Typora/typora-user-images/image-20250717144503668.png)                                                   

### **字典(dict)**：

另一种可变容器模型，且可存储任意类型对象。字典的每个键值 **key:value** 对用冒号 **:** 分割，每个键值对之间用逗号 **,** 分割，整个字典包括在花括号 **{}** 中 ,格式如下所示：`d = {key1 : value1, key2 : value2 }`‘

->字典值可以没有限制地取任何 python 对象，既可以是标准的对象，也可以是用户定义的，但键不行。

两个重要的点需要记住：

1）不允许同一个键出现两次。创建时如果同一个键被赋值两次，后一个值会被记住

2）键必须不可变，所以可以用数字，字符串或元组充当，所以用列表就不行

<img src="/home/wybie/.config/Typora/typora-user-images/image-20250717144915800.png" alt="image-20250717144915800" style="zoom:80%;" />

- **try-except-else-finally语句**：try语句用于捕获和处理程序运行时可能出现的异常，从而提高程序的健壮性和稳定性。异常是指程序在运行过程中遇到的错误，常见的异常类型包括*ValueError*、*TypeError*、*FileNotFoundError*等

```
try:
num = int(input('请输入一个整数:'))
result = 8 / num
except ZeroDivisionError:
print('0不能做除数')
except ValueError:
print('输入的值不是合法的整数')
else:
print(f'结果是: {result}')
finally:
print('程序执行完毕')
```

- **pipeline(管道)：**

  管道函数采用一个初始值和一系列函数，并将每个函数应用于前一个函数的输出，返回最终结果。例如:

  ```cpp
  from toolz.curried import pipe,map,filter
  
  numbers = [1,2,3,4,5,6,7,8,9,10]
  average = pipe(
      numbers,
      filter(lambda  n: n%2==0),
      map(lambda  n: n * 10),
      map(lambda  n: n + 5),
      list,
      lambda x: sum(x)/len(list(x)),
  )
  
  print(average)
  ```

  这段代码比之前的代码可读性更强，也更优雅。它清楚地显示了应用于数据的操作序列，并且不使用任何嵌套调用或中间列表。管道函数使代码看起来像一个管道，使得数据从一个函数流到下一个函数。

**lambda用于创建匿名函数，适合简单逻辑；map对序列元素执行操作；filter按条件筛选元素；reduce累积计算序列元素**

- numpy数组：

  NumPy库的*np.array*函数用于创建数组

	**数据类型**: 可以通过*dtype*参数指定数组的数据类型。如果不指定，		    NumPy会自动选择合适的类型。

	**形状**: 数组的形状可以通过*.shape*属性获得，也可以使用*.reshape()*方法改变形状。

	**维度**: 可以通过*ndmin*参数指定生成数组的最小维度。

```
# 基本运算
e = np.array([10,20,30,40])
f = np.arange(4)
print(e-f) # 输出: [10 19 28 37]
print(e*f) # 输出: [ 0 20 60 120]

# 矩阵乘法
g = np.array([[1,2],[3,4]])
h = np.array([[5,6],[7,8]])
print(g.dot(h)) # 输出:
# [[19 22]
# [43 50]]
```

->`if __name__ == '__main__':` 是 Python 中一个常见的代码结构，它的作用是**判断当前脚本是否是直接运行的**（而不是被其他脚本导入的）

深度相机https://blog.csdn.net/doudou2weiwei/article/details/139934114