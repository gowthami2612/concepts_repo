## 1.What is the difference between (==) and (===) operator ?

- The == is called the abstract equality operator it returns true if the both operators are same value. the === is called as the strict equality operator. it returns true if the both operands are of the same type and same value.
--
### 2.Console.log(typeof []) is equals to 'object' why?

- In JavaScript, `typeof []` is `'object'` because arrays are a type of object.
--

## 3.Whats are the disadvantages of using closure

- the main disadvantages in the closure are the memory usage is more and the debugging is also difficult.
--
## 4.Why using global variables are bad in js ?

- using global variables is bad because they can lead to namespace collisions and unindented side eddects making code harder to maintain and debug.


## 5.How to extract certain properties from an array of objects to create a new array ?

- we can use the map() to extract certain properties from an array of objects to create a new array.
  
--

## 6.Difference between charAt() and at() method in js ?

- charAt returns the character at the specified index in the string.at() is a method is available for accessing elements at a specific index in arrays but not in strings.
--
## 7.How to reset initial or 1st commit in git, if its possible ?

-    It is not possible to revert the first commit instead we can create a new branch make changes and commit and delete the old one.

--
## 8.console.log(typeof []) returns 'object', then why can not we use (.) operator in array to accesss its values just like objects,where we use (.) operator in objects for accessing key and values

- In JavaScript, arrays are a special type of object where keys are automatically assigned as indices, hence we access their values using square brackets to define an index
--

## 9. Why 'forEach' loop skips 'not defined' whereas 'for' loop gives 'undefined' ?

- The `forEach` loop skips over elements that are `undefined` or `not defined`, whereas a `for` loop explicitly returns `undefined` when accessing such elements in JavaScript.
--

## 10.How can we mimic the action Array.splice and 'Array.slice' on objects

- You can't directly mimic `Array.splice` and `Array.slice` actions on objects in JavaScript like you can with arrays.
--
## 11.What is "Callback Hell" problem and how to avoid it ?

-callback hell is a situation where one callback function calls another callback and so on. To avoid this we can use promises.

--

## 12. Question
//file1.js
let ar = [1,2,3];
console.log("Hello");
module.exports.ar = ar;

//file2.js
const {ar} = require('file1.js');
let print = ar;
console.log(print);

Output: "Hello" 
                [1,2,3]
why "Hello" is also printing ? when we have exported array('ar') only!

-"Hello" is printed because `console.log("Hello");` in `file1.js` runs when `file1.js` is required, executing all top-level code including console outputs.

