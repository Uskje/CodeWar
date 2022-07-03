# CodeWars Python Solutions

---

## L1: Set Alarm


Write a function named setAlarm which receives two parameters. The first parameter, employed, is true whenever you are employed and the second parameter, vacation is true whenever you are on vacation.

The function should return true if you are employed and not on vacation (because these are the circumstances under which you need to set an alarm). It should return false otherwise.


---

### Given Code

```python
def set_alarm(employed, vacation):
```
---

### Solution

```python
def set_alarm(employed, vacation):
   return True if employed and not vacation else False
```

-------

[See on CodeWars.com](https://www.codewars.com/kata/568dcc3c7f12767a62000038/train/python)
