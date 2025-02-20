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

## Количество доступных ячеек называют размером или длиной массива. В JavaScript длина массива обычно совпадает с количеством элементов в нем. Массивы хранят свой размер в свойстве ``` length ```:
```js
const infoArray = [
  'Россия', 'Москва', 144.5, 'Russian ruble', true
]
console.log(infoArray.length)
// 5
```
