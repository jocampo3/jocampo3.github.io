```javascript
function insertionSort(arr) {
  for (let i = 1; i < arr.length; i++) {
    let key = arr[i];
    let j = i - 1;
    while (j >= 0 && arr[j] > key) {
      arr[j + 1] = arr[j];
      j = j - 1;
    }
    arr[j + 1] = key;
  }
  return arr;
}

let arr = [9, 1, 8, 2, 7, 3, 6, 5, 4];
sortedArr = insertionSort(arr);
console.log(sortedArr);
```
