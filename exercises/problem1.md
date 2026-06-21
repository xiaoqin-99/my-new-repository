# Problem 1 — 阶乘函数

描述：实现一个函数 factorial(n)，返回 n 的阶乘（非负整数）。

要求：
- 支持 n = 0 返回 1
- 若 n 为负数，抛出 ValueError

示例（Python）：

```python
def factorial(n):
    if n < 0:
        raise ValueError("n must be non-negative")
    if n == 0:
        return 1
    result = 1
    for i in range(1, n+1):
        result *= i
    return result
```
