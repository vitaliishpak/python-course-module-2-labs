##Laboratory Work 2.2

####Description:

Write the code to perform following task:

- Generate sequence 5 integers long from range(0, 100)
- Generate random float
- Print variables above
- Find max element from generated sequence
- Make a floor division between max element and generated float
- Find factorial of the result above
- Shorten the code as much as possible

####Here is its solution code:

*solution_2_2.py*
```python
import random
import math

"""Generate sequence 5 integers long from range(0, 100)
"""
integers_sequence = random.sample(range(100), 5)
print('5 integers from range(0, 100): {}'.format(integers_sequence))

"""
Generate random float
"""
generated_float = random.random()

"""
Print variables above
"""
print('random float: {}'.format(generated_float))

"""
Find max element from generated sequence
"""
max_in_sequence = max(integers_sequence)
print('max element from generated: {}'.format(max_in_sequence))

"""
Make a floor division between max element and generated float
"""
floor_division = max_in_sequence // generated_float
print('floor division between max element and generated float: {}'.format(floor_division))

"""
Find factorial of the result above
"""
print('factorial of the result above: {}'.format(math.factorial(floor_division)))

"""
Shorten the code as much as possible
"""

```
