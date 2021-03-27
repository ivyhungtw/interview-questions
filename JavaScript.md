# Backend Interview Question - (4) JavaScript

## Keywords
- DOM
- Unobtrusive JavaScript
- prototype
- bind
- call
- Prototypal inheritance
- Scoping
- Closure
- The event loop
- Event bubbling
- Apply, call, and bind
- Callbacks and promises
- Variable and function hoisting
- Currying
- apply
- map
- event delegation
- ajax

## JavaScript
### 1. What is the value of foo.length?
```
var foo = [];
foo.push(1);
foo.push(2);
```
### 2. Which is equal to the condition？
```
if (ua !== 'IE 6'&& ua !== 'IE 7')
A. if (ua === 'IE 6' || ua === 'IE 7')
B. if (ua === 'IE 6' && ua === 'IE 7')
C. if (! (ua === 'IE 6'|| ua === 'IE 7'))
D. if (! (ua === 'IE 6'&& ua === 'IE 7'))
```
### 3. Which is true ?
```
A. 1 === true
B. Number('1px')
C. typeof [1, 2, 3] == 'array'
D. '0'
E. None of the above
```
### 4. What is b :
```
var a = [ 1, 2, 3 ];
var b = a;
a.push(5);
console.log(b)
```
### 5. How can we get the 'hello':
```
var obj = { 1: 'hello', 2: 'world'}
```
A. `obj.1`
B. `obj[0]`
C. `obj[1]`
D. `obj.2`

### 6. Please answer all below typeof:
`typeof function(){}`
`typeof new Date()`
`typeof {}`
`typeof new Array()`

### 7. Please explain what is the difference between `setTimeout()` and `setInterval()` ?
### 8. Please explain what the use of `preventDefault()` and `stopPropagation()` in Event Object ?
### 9. 怎樣添加、移除、移動、複製、創建和查找節點？
### 10. 實現一個函數 clone，可以對 JavaScript 中的 5 種主要的數據類型（包括 Number、String、Object、Array、Boolean）進行值複製。
### 11. 如何消除一個數組裡面重複的元素？
### 12. 在 Javascript 中什麼是偽數組？如何將偽數組轉化為標準數組？（Array and Key-value Pair）
### 13. Javascript 中 callee 和 caller 的作用？
### 14. 請描述 cookies，sessionStorage 和 localStorage 的區別。
### 15. 請描述 web storage 和 cookie 的區別。
### 16. 請你實踐一個可以統計字串中字母個數或統計最多字母數的涵式。
### 17. Use recursion to log a fibonacci sequence of n length.
### 18. Walk us through the process of creation of an application or website you've built.
### 19. What are the differences between functional and imperative programming styles, and explain your preference, if any.
### 20. What is the significance, and what are the benefits, of including `'use strict'` at the beginning of a JavaScript source file?
### 21. What is `NaN`? What is its type? How can you reliably test if a value is equal to `NaN`?
### 22. Discuss possible ways to write a function `isInteger(x)` that determines if x is an integer.
### 23. In what order will the numbers 1-4 be logged to the console when the code below is executed? Why?
```
(function() {
    console.log(1); 
    setTimeout(function(){console.log(2)}, 1000); 
    setTimeout(function(){console.log(3)}, 0); 
    console.log(4);
})();
```
### 24. Explain how `this` works in JavaScript
### 25. Explain why the following doesn't work as an IIFE: `function foo(){ }()`;.
### 26. What needs to be changed to properly make it an IIFE?
### 27. What's the difference between a variable that is: `null`, `undefined` or `undeclared`?
### 28. How would you go about checking for any of these states?
### 29. Can you describe the main difference between a `forEach` loop and a `.map()` loop and why you would pick one versus the other?
### 30. How do you organize your code? (module pattern, classical inheritance?)
### 31. Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
### 32. What's the difference between .call and .apply?

## jQuery
### 1. 什麼是 jQuery？請寫出一段 jQuery code 可以點擊一個按鈕後，動態插入 HTML 元素。
### 2. jQuery 中的 `$(document).ready` 方法是什麼作用？
### 3. jQuery 的事件委托方法 on、live、delegate 之間有什麼區別？