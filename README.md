# ARR (Array)
## ARR — Массив — это структура, в которой можно хранить коллекции элементов — чисел, строк, других массивов и так далее

## Массивы очень похожи на нумерованные списки.

---

# Как пишем:
## Создадим массив с помощью квадратных скобок [].

## К примеру, можно создать пустой массив:
``` js 
const guestList = [] // 😭 гостей нет
```
## А можно создать сразу с элементами внутри:

``` js 
const theGirlList = [
  'Серсея', 'Илин Пейн', 'Меррин Трант', 'Дансен', 'Гора'
]
```

## Элементы могут быть разных типов:

``` js 
const infoArray = [
  'Россия', 'Москва', 144.5, 'Russian ruble', true
]
```

## Внутри массива могут быть другие массивы:

```js 
const arrayOfArrays = [
  'Россия',
  ['Москва', 'Санкт-Петербург', 'Казань', 'Екатеринбург'],
  [true, true, false, true]
]
```
---

## Количество доступных ячеек называют _размером_ или _длиной_ массива. В JavaScript длина массива обычно совпадает с количеством элементов в нем. Массивы хранят свой размер в свойстве ``` length ```:
```js
const infoArray = [
  'Россия', 'Москва', 144.5, 'Russian ruble', true
]
console.log(infoArray.length)
// 5
```
# JS Mechanism
***As you probably heard, JavaScript is a single-thread programming language. It means processed operations are handled one by one. JavaScript doesn’t have the ability to make operations parallel. We can do it in a programming language like Java, where we have the possibility to run several calculations in multiple threads. JavaScript cannot do that, it processes all the operations in sequence, so it might be very slow. But it isn’t! All of you are using very complex websites and huge web applications like Facebook. At the same time, the browser is downloading posts into our wall, we are writing and sending messages, displaying our friends’ images, clicking “Like” under them, and we don’t have any delays. It is all because of the mechanism called EventLoop***

<details>
    <summary>Destructuring assignment</summary>
    <br>

***The destructuring assignment syntax is a JavaScript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables***
<br>

```javascript 

let a , b  , rest 
[ a , b ] = [ 10 , 20 ]

console.log(a) //10
console.log(b) //20

[ a , b , ...rest] = [10 , 20 , 30 , 40 , 50]
console.log(rest) // [30 , 40 , 50]
```
<br>

</details>

<details>
    <summary>Spread syntax(...)</summary>

***Spread syntax can be used when all elements from an object or array need to be included in a new array or object, or should be applied one-by-one in a function call's arguments list***
<br>

```js
let arr = [ 1 , 2 , 3 ]
let arr2 = [...arr]

arr2.push(4)
console.log(arr2) // [1 , 2 , 3 , 4]
console.log(arr) // [1 , 2 , 3]
```
<br>
</details>

<details>
    <summary>Rest</summary>

***The rest parameter syntax allows a function to accept an indefinite number of arguments as an array, providing a way to represent variadic functions in JavaScript.***
<br>

```js
function myFun(a, b, ...manyMoreArgs) f console.log("a", a); console.log("b", b); console.log("manyMoreArgs" manyMoreArgs); Y
 myFun ("one"
"tWo"
"three", "four", "five", "six");
// Console Output: 1 a, one 1 b tWO // manyMoreArgs
 ["three" "four" "five", "six"]
```
 
</details>
```
