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

# LEVEL 3 Работа с функциями

Стрелочная функция
```js
const arrayFunction = (message) => {
    return message.reverse()
};

console.log(arrayFunction('hello, world')) //dlrow ,ollhe
```

Callback функция

```js
const func = (callback) => {
    callback('hello, world');
}

func((message) => console.log(message)) //hello, world
```

# LEVEL 3 DOM
Тут тебе нужно разбираться самостоятельно. Маленькая подсказка:
```js
appendChild()
```

# LEVEL 3 NODE.JS

Выполнить файл index.js с таким кодом в среде node.js:

```js
const msg = 'hello, world'
console.log(msg);
```
Для того чтобы выполнить такой код, нужно написать
в терминале: 

```bash
$ node index.js
```

Добавить npm в свой проект
```bash
$ npm init
```

Установка пакета через npm:
```bash
$ npm install <название пакета>
```

Как создать сервер на express.js
```text
ОТКРЫВАЙ ИХ ДОКУМЕНТАЦИЮ И ЧИТАЙ. ТАМ ВСЕ ПРОСТО
```

#
Установка MongoDB:
```bash
$ sudo apt install mongodb-server-core
$ sudo apt install mongodb-clients
```
Затем в папке home в терминале написать, 
```bash
$ sudo mkdir -p /data/db
$ sudo mongod 
```
Эта команда запускает сервер MongoDB у тебя на компьютере.
##

Запустить клиент MongoDB для работы с ней:
```bash
$ mongo
```
##

Когда запустил клиент, открывай документацию MongoDB, и читай как она работает.
```js
db.<имя коллекции>.insertOne({name: 'Misha', age: 20}); // добавить запись в коллекцию
db.<имя коллекции>.findOne({name: 'Misha'}); //найти одну запись в коллкции
db.<имя коллекции>.find({age: 20}); // найти все записи в коллекции с age: 20
db.<имя коллекции>.remove({}); // удалить элементы из коллкции
use <имя базы данных> // выбрать базу данных
show collections // показать все коллекции
```

