```ruby
def insertion_sort(a)
  return "Elements sorted" if a.count <= 1

  arr_range = a.count - 1
  for i in 1..arr_range do
    key = a[i]
    j = i - 1
    while j >= 0 && a[j] > key
      a[j + 1] = a[j]
      j = j - 1
    end
    a[j+ 1] = key
  end

  return a
end

a = [5, 2, 4, 6, 1, 3]
sorted = insertion_sort(a)
puts sorted
```
