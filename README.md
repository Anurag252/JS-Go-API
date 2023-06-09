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

## Strings
|   |  Go |  JS | 
|---|---|---|
| char or string at an index | string(str[index]) | `str.at(index)`  | 
| ascii value of char | int(string(str[index])) | `str.charCodeAt(index)`  | 
| concat string | use sprintf or `strings.Join([]str, sep)` | `str.concat(index)`  | 
| string ends with | `strings.HasSuffix("foobar", "bar")` | `str1.endsWith(str2)`  | 
| string contains another substring | `strings.Contains(str, substr string)` | `str.includes(index)`  | 
| index of another substring | `strings.Index(s, substr)` | `str.indexOf(anotherstr)`  | 
| replace or replace all occurences | strings.Replace("","") | `str.replace("k","")`  | 
| match regex | string(str[index]) | `str.search(regex)`  | 
| substring | str[a:b] | `str.slice()`  | 
| split | strings.split() | `str.split()`  | 
| trim string | strings.Trim(s, cutset string) | `str.Trim()` // remove leading and trailing spaces | 

Numbers
-------

|  | Go | JS |
| --- | --- | --- |
| absolute value | `math.Abs(num)` | `Math.abs(num)` |
| random number between 0 and 1 | `rand.Float64()` | `Math.random()` |
| round to nearest integer | `math.Round(num)` | `Math.round(num)` |
| convert string to integer | `strconv.Atoi(str)` | `parseInt(str)` |
| convert string to float | `strconv.ParseFloat(str, 64)` | `parseFloat(str)` |
| convert integer to string | `strconv.Itoa(num)` | `num.toString()` |
| convert float to string | `strconv.FormatFloat(num, 'f', 2, 64)` | `num.toString()` |
| infinity | `math.Inf(1)` | `Infinity` |

Booleans
--------

|  | Go | JS |
| --- | --- | --- |
| boolean not | `!a` | `!a` or `a = !a` |
| boolean and | `a && b` | `a && b` |
| boolean or | `a || b` | `a || b` |

Objects
-------

|  | Go | JS |
| --- | --- | --- |
| create empty object | `make(map[string]interface{})` | `{}` |
| get value of key in object | `obj["key"]` | `obj.key` or `obj["key"]` |
| set value of key in object | `obj["key"] = val` | `obj.key = val` or `obj["key"] = val` |
| delete key in object | `delete(obj, "key")` | `delete obj.key` or `delete obj["key"]` |
| check if object has key | `_, ok := obj["key"]` | `"key" in obj` or `obj.hasOwnProperty("key")` |

Dates
-----

|  | Go | JS |
| --- | --- | --- |
| get current date and time | `time.Now()` | `new Date()` |
| format date to string | `time.Now().Format("02-Jan-2006")` | `new Date().toLocaleDateString('en-US', { year: 'numeric', month: 'short', day: '2-digit' })` |
| add or subtract time to date | `time.Now().AddDate(0, 0, 1)` or `time.Now().Add(time.Hour)` | `new Date(Date.now() + 86400000)` or `new Date().setDate(new Date().getDate() + 1)` |

Regular Expressions
-------------------

|  | Go | JS |
| --- | --- | --- |
| create regular expression object | `regexp.MustCompile("pattern")` | `/pattern/` |
| test if string matches pattern | `regexp.MustCompile("pattern").MatchString(str)` | `/pattern/.test(str)` |
| find first match of pattern in string | `regexp.MustCompile("pattern").FindString(str)` | `str.match(/pattern/)[0]` |

Promises and Asynchronous Programming
-------------------------------------

|  | Go | JS |
| --- | --- | --- |
| create a promise | `funcName() (result, error)` | `new Promise((resolve, reject) => {})` |
| resolve a promise |  |  |

