# JS-Go-API

|   |  Go |  JS | 
|---|---|---|
| Do a substring  |  `str[a:b]` | `str.subString(startindex, lengthfromstart)`  | 
| create a subarray  | `arr[a:b]`  | `arr.slice(start, end+1)` // as endindex is not included | 
| join array  | `arr := append(arr1, arr2)` | `arr = arr1.concat(arr2)`  | 
| item at index  | `arr[index]` | `arr.at(index) ` | 
| concat string  | `fmt.Sprintf("%v %v",str1, str2)` | `${str1} ${str2}`  | 
| test if all array elements pass a test  | `for i,v := range arr { if !test(v) { return false}}` | `arr.every((x) => test(x))` // implicit return  | 
| fill an array with static value | loop over array | `array1.fill(5, 1)` // fill 5 from position 1  | 
| filter using some condition  | loop over array and append | arr.filter((x) => returnsbool(x)) // returns a filtered value  | 
| find  | loop over array | `arr.find((x) => )` // returns first element also findIndex, findLast, findLastIndex | 
| flat an array | use loop and recursion 👿  | `[0, 1, 2, [3, 4]].flat()` or `arr1.flatMap((num) => (num === 2 ? [2, 2] : 1))` // same as map and then flat | 
| convert from iterable to array | for range will loop , then append| Array.from(iterable) | 
| group array by some  |   |  🚧 see group or groupToMany  | 
| contains in array | loop and find  | `[0, 1, 2].includes()` // returns boolean  | 
| find index of  | use loop and return index  | `[0, 1, 2].indexOf(2)`  | 
| join elements of array | use loop and use string builder | `[0, 1, 2].join()`  | 
| transform array | use loop  | `[0, 1, 2].map()`  | 
| add to an array | arr = append(arr,elem) | `[0, 1, 3].push()`  | 
| remove from an array | arr = arr[:b] | `[0, 1, 3].pop()`  | 
| sum all elements of array | loop and sum | `const sumWithInitial = array1.reduce(
  (accumulator, currentValue) => accumulator + currentValue,
  initialValue
);`  | 
| reverse an array | use two pinter and swap | `[0, 1, 3].reverse()` to do without mutating array use `.toReversed()() | 
| at least one array satisfies condition | loop and test a condition | `[0, 1, 3].some()`  | 
| in place sort | sort.Ints(arr) | `[0, 1, 3].sort()` to do without mutating array use `.toSorted() | 
| add to an array | arr = append(arr,elem) | `[0, 1, 3].push()`  | 
| add to an array | arr = append(arr,elem) | `[0, 1, 3].push()`  | 
| add to an array | arr = append(arr,elem) | `[0, 1, 3].push()`  | 
| add to an array | arr = append(arr,elem) | `[0, 1, 3].push()`  | 
