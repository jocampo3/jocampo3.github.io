```go
package main

import "fmt"

func insertion_sort(a []int) {
	if len(a) <= 1 {
		return
	}

	for i := 1; i < len(a); i++ {
		key := a[i]
		j := i - 1
		for j >= 0 && a[j] > key {
			a[j+1] = a[j]
			j--
		}

		a[j+1] = key
	}
}

func main() {
	var a = []int{5, 2, 4, 6, 1, 3}
	insertion_sort(a)
	fmt.Println(a)
}
```
