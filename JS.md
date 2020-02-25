# LEVEL 1

Создать переменную - 
```js
const variable = 10;
const variable = 'строка';
let variable = 10;
let variable = 'строка';
```
переменные типа let можно изменять после создания

const - изменять нельзя

#


Вывод в консоль -
```js
console.log('привет как дела');
```

Ветвление в js - 
```js
let variable = 10;

if (variable==10) {
    variable+=1;
}
```

Циклы в js -
```js
for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

Создать массив - 
```js
const array = [];
```

Добавить элемент в массив -
```js
const variable = 10;
const array = [];

array.push('10');
array.push(variable);
```

Вывести все элементы массива - 
```js
const variable = 10;
const array = [];

array.push('10');
array.push(variable);

array.forEach(element => console.log(element));
```

если чет непонятно будет - пиши, спрашивай

# LEVEL 2

функция map делает из массива другой массив, например
```js
const a = [1, 2, 3, 4, 5, 6]
const b = a.map((element)=>element*2)
console.log(b); // [2, 4, 6, 8, 10, 12]
```

структура обьекта в js

```js
const a = {
    ключ: 'значение'
}
```
достать из обьекта значение по его ключу
```js
const a = {
    field: 'value'
}

console.log(a.field); // value
console.log(a['field']) // value

```
 # LEVEL 2 DOM
 
 Достать элементы из DOM по его ID
 
 ```html
<div id="privetkakdela">kolyaaaan</div>
```
 ```js
const a = document.getElementById('privetkakdela');
console.log(a.innerHTML) // kolyaaaan
```

#
Функция для кнопок 

```js
function f() {
  console.log('privet');
}
```

```html
<button onclick="f()">press me</button>
```
#
Текст из input

```html
<input id="fed"/>
```

```js
const inputik = document.getElementById('fed');

inputik.addEventListener('input', function(e) {
  console.log(e.target.value); //выводит содержание input после любого его изменения
});
```
#
На каких координатах в DOM находится текущий scroll
```js
window.scrollY+window.innerHeight
```

event для scroll'а 

```js
window.addEventListener('scroll', function() {
    
});

```
координаты по Y любого элемента

```js
  const a = document.getElementById('test');
  console.log(a.offsetTop);
```
