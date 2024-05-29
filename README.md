# Re:0 从零开始的Python学习生活

```python
#创建列表，元素为 12, 17, 28, 19, 11，并赋值给 numbers 变量
numbers = [12, 17, 28, 19, 11]

#使用列表推导创建一个新的列表只包含奇数
odd_numbers = [num for num in numbers if num % 2 != 0]

#打印新创建的列表
print(odd_numbers)
```


```python
#创建lambda函数，返回参数的立方 
get_cube = lambda number:number**3

#输入一个整数 
number = int(input())

#调用函数并打印结果 
print(get_cube(number))
```


```python
def multiply_numbers(*args):
#如果没有传入参数，则返回1（乘法单位元）
    if not args:
        return 1
    
    product = 1
    for num in args:
        product *= num
    return product

#输入三个整数
num1 = int(input("请输入第一个整数: "))
num2 = int(input("请输入第二个整数: "))
num3 = int(input("请输入第三个整数: "))

#用这三个整数调用multiply_numbers()函数并打印返回值
result = multiply_numbers(num1, num2, num3)
print("乘积是:", result)
```
****args 是一种用于在函数中处理可变数量参数的语法。*args 允许你传递任意数量的非关键字参数给一个函数。***


```python
#创建函数，参数为可变数量的关键字参数
def full_name(**kwargs):
    # 打印参数
    print(kwargs)

#输入第一个名字
first = input("请输入第一个名字: ")
# 输入最后一个名字
last = input("请输入最后一个名字: ")

#调用函数，用输入的名字作为关键字参数
full_name(first=first, last=last)
```
输出
```python
请输入第一个名字: John
请输入最后一个名字: Doe
{'first': 'John', 'last': 'Doe'}
```
