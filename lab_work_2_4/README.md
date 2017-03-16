##Laboratory Work 2.4

####Description:

Write the code to do following:
- Generate list with lowercase and uppercase alphabet plus numbers
- Print 1st symbol of list
- Print last symbol
- Print 3rd from start and 3rd from the end
- Slice first 10 symbols
- Print only symbols with index, which divides on 2 without remaining
- Print only integer values from list
- Reverse list using slice
- Convert base list into string

####Here is its solution code:

*solution_2_4.py*
```python
z = ['Main', 'A', 'c', 'a', 'd', 'e', 'm', 'y', 2, 0, 1, 7]

"""Generate list with lowercase and uppercase alphabet plus numbers
"""
print(z)

"""Print 1st symbol of list
"""
print(z[0])

"""Print last symbol
"""
print(z[-1])

"""Print 3rd from start and 3rd from the end
"""
print(z[2], z[-3])

"""Slice first 10 symbols
"""
print(z[:10])

"""Print only symbols with index, which divides on 2 without remaining
"""
print(z[2:len(z):2])

"""Print only integer values from list
"""
x = str(z)
digits = []
for symbol in x:
    if '1234567890'.find(symbol) != -1:
        digits.append(int(symbol))
print(digits)

"""Reverse list using slice
"""
print(z[::-1])

"""Convert base list into string
"""
print(str(z))

```