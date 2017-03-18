##Laboratory Work 2.6

####Description:

Write the code to do following:

- Generate two sets with not unique numbers and few symbols
- Print 1st set
- Create tuple from intersection of first and second set
- Create tuple from difference first and second set
- Slice first 3 symbols from first tuple
- Print only symbols with numbers from second set
- Reverse tuple using slice
- Convert both tuples into list

####Here is its solution code:

*solution_2_6.py*
```python
"""Generate two sets with not unique numbers and few symbols
"""
x = set('Live77abc88-terracotta')
y = set('Love17milan70-evolution')

"""Print 1st set
"""
print('Set 1: {}'.format(x))
print('Set 2: {}'.format(x))

"""Create tuple from intersection of first and second set
"""
t1=tuple(x & y)
print('Tuple from intersection of first and second set: {}'.format(t1))

"""Create tuple from difference first and second set
"""
t2=tuple(x - y)
print('Tuple from difference first and second set: {}'.format(t2))

"""Slice first 3 symbols from first tuple
"""
print('Slice first 3 symbols from first tuple: {}'.format(t1[:3]))

"""Print only symbols with numbers from second set
"""
for s in y:
    try:
        print('Symbols with numbers from second set: {}'.format(int(s)))
    except ValueError:
        pass

"""Reverse tuple using slice
"""
print('Reverse tuple 1: {}'.format(t1[::-1]))
print('Reverse tuple 1: {}'.format(t2[::-1]))

"""Convert both tuples into list
"""
print('Convert tuple 1 into list 1: {}'.format(list(t1)))
print('Convert tuple 2 into list 2: {}'.format(list(t2)))

```