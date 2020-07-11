<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png"> 
  <h1>JavaScript Shorts</h1>
  
  [![GitHub license](https://img.shields.io/github/license/aniketkudale/JavaScript-Shorts)](https://github.com/aniketkudale/JavaScript-Shorts/blob/master/LICENSE) [![GitHub stars](https://img.shields.io/github/stars/aniketkudale/JavaScript-Shorts)](https://github.com/aniketkudale/JavaScript-Shorts/stargazers) [![GitHub forks](https://img.shields.io/github/forks/aniketkudale/JavaScript-Shorts)](https://github.com/aniketkudale/JavaScript-Shorts/network) [![GitHub issues](https://img.shields.io/github/issues/aniketkudale/JavaScript-Shorts)](https://github.com/aniketkudale/JavaScript-Shorts/issues) ![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Faniketkudale%2FJavaScript-Shorts) ![GitHub followers](https://img.shields.io/github/followers/aniketkudale?style=social)

<span>A crowd sourced list of short essential JavaScript snippets. <span>

---

</div>

## Table of Contents

1. **[Check if value is a Number](#1-check-if-value-is-number)**
2. **[Check if value is in Array or String](#2-check-if-value-is-array-or-string)**
3. **[Create an Array from a String](#3-check-an-array-from-a-string)**
4. **[Check if Array](#4-check-if-Array)**
5. **[Merge Two Arrays](#5-merge-two-arrays)**
6. **[Copy a value within Array](#6-copy-a-value-within-array)**
7. **[Return Array iterator](#7-return-array-iterator)**
8. **[Check if all elements pass test](#8-Check-if-all-elements-pass-test)**
9. **[Fill an array with a static value](#9-Fill-an-array-with-a-static-value)**
10. **[Filter an Array](#10-filter-an-array)**
11. **[Find in an Array](#11-find-in-an-array)**
12. **[Flatten an Array](#12-flatten-an-array)**
13. **[Array forEach()](#13-array-foreach)**
14. **[Array indeOf()](#14-array-indeof)**

---

## 1. Check if value is number
```javascript
//using isNaN()
const value = 3

isNaN(value) //false
isNaN('string') //true

//using typeof
typeof 1 //'number'

//using conditional check
if (typeof value === 'number') {
	//its a number
}
```

## 2. Check if value is Array or String
```javascript
const array = [1, 2, 3];

console.log(array.includes(2)) // true

const fruits = ['apple', 'orange', 'banana'];

console.log(fruits.includes('apple')) // true

console.log(fruits.includes('range')) // false

const str = "Hello World"; // With String

console.log(str.includes('o W')) // true
```

## 3. Create and Array from a string
```javascript
console.log(Array.from('foo'));
// expected output: Array ["f", "o", "o"]

console.log([...'foo']);
// expected output: Array [2, 4, 6]
```

## 4. Check if Array
```javascript
Array.isArray([1, 2, 3]);  // true
Array.isArray({foo: 123}); // false
Array.isArray('foobar');   // false
Array.isArray(undefined);  // false
Array.isArray('foo'.split('')); // true
```

## 5. Merge two Arrays
```javascript
const teamCaptainAmerica = ['Captain America', 'Bucky Barnes', 'Falcon', 'Scarlet Witch', 'Hawkeye', 'Ant-Man'];
const teamIronMan = ['Iron Man', 'Black Panther', 'Vision', 'Black Widow', 'War Machine', 'Spider-Man'];
const avengers = teamCaptainAmerica.concat(teamIronMan);

console.log(avengers);
/* 
  output: Array ["Captain America", "Bucky Barnes", "Falcon", "Scarlet Witch", 
 "Hawkeye", "Ant-Man", "Iron Man", "Black Panther", "Vision", "Black Widow", "War Machine", "Spider-Man"] 
*/

```

## 6. Copy a value within Array
```javascript
const array1 = ['a', 'b', 'c', 'd', 'e'];

// copy to index 0 the element at index 3
console.log(array1.copyWithin(0, 3, 4));
// expected output: Array ["d", "b", "c", "d", "e"]

// copy to index 1 all elements from index 3 to the end
console.log(array1.copyWithin(1, 3));
// expected output: Array ["d", "d", "e", "d", "e"]

```

## 7. Return Array iterator
```javascript
const array1 = ['a', 'b', 'c'];

const iterator1 = array1.entries();

console.log(iterator1.next().value);
// expected output: Array [0, "a"]

console.log(iterator1.next().value);
// expected output: Array [1, "b"]

```

## 8. Check if all elements pass test
```javascript
const isBelowThreshold = (currentValue) => currentValue < 40;

const array1 = [1, 30, 39, 29, 10, 13];

console.log(array1.every(isBelowThreshold));
// expected output: true

```

## 9. Fill an array with a static value
```javascript
const array1 = [1, 2, 3, 4];

// fill with 0 from position 2 until position 4
console.log(array1.fill(0, 2, 4));
// expected output: [1, 2, 0, 0]

// fill with 5 from position 1
console.log(array1.fill(5, 1));
// expected output: [1, 5, 5, 5]

console.log(array1.fill(6));
// expected output: [6, 6, 6, 6]

```

## 10. Filter an array
```javascript
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

// Return new array
const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]
```

## 11. Find in an array
```javascript
const array1 = [5, 12, 8, 130, 44];

const found = array1.find(element => element > 10);

console.log(found);
// expected output: 12
```

## 12. Flatten an array
```javascript
const arr = [1, 2, [3, 4]];

// To flat single level array
arr.flat();
// is equivalent to
arr.reduce((acc, val) => acc.concat(val), []);
// [1, 2, 3, 4]

// or with decomposition syntax
const flattened = arr => [].concat(...arr);
// expected output: 12
```
## 13. Array forEach()
```javascript
// The forEach() method executes a provided function once for each array element.
const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

// expected output: "a"
// expected output: "b"
// expected output: "c"

```

## 14. Array indeof()
```javascript
const beasts = ['ant', 'bison', 'camel', 'duck', 'bison'];

console.log(beasts.indexOf('bison'));
// expected output: 1

// start from index 2
console.log(beasts.indexOf('bison', 2));
// expected output: 4

console.log(beasts.indexOf('giraffe'));
// expected output: -1

```
