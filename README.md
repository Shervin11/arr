# ARR (Array)
## ARR — Массив — это структура, в которой можно хранить коллекции элементов — чисел, строк, других массивов и так далее
## Массивы очень похожи на нумерованные списки.

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

## 

```js
import { sort, filter, map } from 'arr';

// Sample array
const numbers = [4, 2, 7, 1, 9, 3];

// Sort the array
const sortedNumbers = sort(numbers);
console.log(sortedNumbers); // Output: [1, 2, 3, 4, 7, 9]

// Filter the array
const filteredNumbers = filter(numbers, num => num > 3);
console.log(filteredNumbers); // Output: [4, 7, 9]

// Map the array
const squaredNumbers = map(numbers, num => num * num);
console.log(squaredNumbers); // Output: [16, 4, 49, 1, 81, 9]
```
