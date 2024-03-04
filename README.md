# Re:0 从零开始的Python学习生活

## 数字类型

```python
import decimal//十以内精确计算
a=decimal.Decimal('0.1')
b=decimal.Decimal('0.2')
print(a+b)

x=1+2j//虚数
x.real//获取实数
x.imag//获取虚数
```

## 数字运算

// 地板除 ***获得比所除结果小的整数***

% 取余***非负数***

divmod 同时得地板除和取余

abs() 取绝对值，取复数的模
