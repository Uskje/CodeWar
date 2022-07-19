# CodeWars Python Solutions

---

## Speed Control


In John's car the GPS records every s seconds the distance travelled from an origin (distances are measured in an arbitrary but consistent unit). For example, below is part of a record with s = 15:
```
x = [0.0, 0.19, 0.5, 0.75, 1.0, 1.25, 1.5, 1.75, 2.0, 2.25]
```
The sections are:
```
0.0-0.19, 0.19-0.5, 0.5-0.75, 0.75-1.0, 1.0-1.25, 1.25-1.50, 1.5-1.75, 1.75-2.0, 2.0-2.25
```
We can calculate John's average hourly speed on every section and we get:
```
[45.6, 74.4, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0, 60.0]
```
Given s and x the task is to return as an integer the *floor* of the maximum average speed per hour obtained on the sections of x. If x length is less than or equal to 1 return 0 since the car didn't move.

Example:
with the above data your function gps(s, x)should return 74
---

### Given Code


```python
def gps(s, x):
  pass
```

---

### Solution


```python
def gps(s, x):
    if len(x) <= 1:
        return 0
    else:
        ht = []
        j = 0
        k = 1
        while k <= len(x)-1:
            dt = (x[k]-x[j])*(3600/s)
            ht.append(dt)
            j += 1
            k += 1
        return int(round(max(ht)))
```


---


[See on CodeWars.com](https://www.codewars.com/kata/56484848ba95170a8000004d/train/python)
