##Laboratory Work 2.3

####Description:

Write the code to do following:

- Generate string with lowercase and uppercase alphabet plus numbers
- Print 1st symbol of string
- Print last symbol
- Print 3rd from start and 3rd from the end
- Slice first 8 symbols
- Print only symbols with index, which divides on 3 without remaining
- Print the symbol of the middle of the string text
- Reverse text using slice

####Here is its solution code:

*solution_2_3.py*
```python
a = 'Barcelona2017'

"""Generate string with lowercase and uppercase alphabet plus numbers
"""
print(a)

"""Print 1st symbol of string
"""
print(a[0])

"""Print last symbol
"""
print(a[-1])

"""Print 3rd from start and 3rd from the end
"""
print(a[2], a[-3])

"""Slice first 8 symbols
"""
print(a[:8])

"""Print only symbols with index, which divides on 3 without remaining
"""
print(a[3:len(a):3])

"""Print the symbol of the middle of the string text
"""
print(a[len(a)//2])

"""Reverse text using slice
"""
print(a[::-1])

```