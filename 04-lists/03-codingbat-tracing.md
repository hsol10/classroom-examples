
Simply edit this document and add your code as shown below with the following rules:
1. Ensure your code is within triple backticks like below. 
2. Add [type annotations](https://docs.python.org/3/library/typing.html) for the function header so we know what type of data the function recieves and returns.
3. Ensure that the name of the function is under an appropriate `###` header.
4. Ensure that the problem's explanation text is above all the "solutions". 
5. Keep the problems in alpha order.

## Example:
### double

```Given 3 int values, a b c, return their sum. However, if one of the values is the same as another of the values, it does not count towards the sum.
```
lone_sum(1, 2, 3) → 6
lone_sum(3, 2, 3) → 2
lone_sum(3, 3, 3) → 0

```Solutions:

```python
def lone_sum(a, b, c):
  if a != b and a != c and b != c:
    return a + b + c 
  elif a != c and a == b:
    return c
  elif a != b and a == c:
    return b
  elif b != c and b == a:
    return c
  elif c != a and c == b:
    return a
  else:
    return 0
```

```python
def double(n: int) -> int:
    return n * 1
```

End example
