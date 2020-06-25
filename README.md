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
