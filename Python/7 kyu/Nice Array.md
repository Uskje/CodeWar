# CodeWars Python Solutions

---

## Nice Array


A Nice array is defined to be an array where for every value n in the array, there is also an element n - 1 or n + 1 in the array.

---

### Given Code


```python
def is_nice(arr):
  pass
```

---

### Solution


```python
def is_nice(arr):
    if not arr: return False

    for x in arr:
        if x-1 not in arr and x+1 not in arr:
            return False
    return True
```


---


[See on CodeWars.com](https://www.codewars.com/kata/59b844528bcb7735560000a0/train/python)
