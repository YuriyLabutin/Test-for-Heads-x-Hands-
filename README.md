# Test-for-Heads-x-Hands-
```python
import random

def generate_sorted_arrays(n):
    arrays = []
    sizes = random.sample(range(1, n * 2), n)
    
    for i in range(n):
        array = random.sample(range(1, 100), sizes[i])
        if i % 2 == 0:
            array.sort()
        else:
            array.sort(reverse=True)
        arrays.append(array)
    
    return arrays
```
