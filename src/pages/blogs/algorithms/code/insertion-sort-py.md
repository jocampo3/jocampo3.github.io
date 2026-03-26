```python
def insertion_sort(a):
    if len(a) <= 1:
        return a

    for j in range(1, len(a)):
        key = a[j]
        i = j - 1
        while i >= 0 and a[i] > key:
            a[i+1] = a[i]
            i = i-1
        a[i+1] = key

    return a

a = [5, 2, 4, 6, 1, 3]

sorted_arr = insertion_sort(a)
print(sorted_arr)
```
