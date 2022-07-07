## Циклы
``` bash
Цикл «while»
    while (condition) {
    // код
    // также называемый "телом цикла"
    }

Цикл «do…while»
    do {
    // тело цикла
    } while (condition);

Цикл «for»
    for (начало; условие; шаг) {
    // ... тело цикла ...
    }
```
## Пример switch case 
``` bash
let result = "";
switch (val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4";
}
```

## Массивы
``` bash
array.push(...items) – добавляет элементы в конец
array.pop() – извлекает элемент из конца
array.shift() – извлекает элемент из начала
array.unshift(...items) – добавляет элементы в начало

array.splice(index[, deleteCount, elem1, ..., elemN]) - начинает с позиции index, удаляет deleteCount элементов и вставляет elem1, ..., elemN на их место. Возвращает массив из удалённых элементов.
array.slice([start], [end]) - возвращает новый массив, в который копирует элементы, начиная с индекса start и до end (не включая end)
array.slice() - без аргументов создаёт копию массива array
array.concat(arg1, arg2...) - создаёт новый массив, в который копирует данные из других массивов и дополнительные значения.
array.forEach - позволяет запускать функцию для каждого элемента массива.
    arr.forEach(function(item, index, array) {
    // ... делать что-то с item
    });
array.indexOf(item, from) – ищет item, начиная с индекса from, и возвращает индекс, на котором был найден искомый элемент, в противном случае -1
array.lastIndexOf(item, from) – то же самое, но ищет справа налево
array.includes(item, from) – ищет item, начиная с индекса from, и возвращает true, если поиск успешен
array.find – item - очередной элемент, index - его индекс, array - сам массив
    let result = arr.find(function(item, index, array) {
    // если true - возвращается текущий элемент и перебор прерывается
    // если все итерации оказались ложными, возвращается undefined
    });
array.filter - ищет один (первый попавшийся) элемент, на котором функция-колбэк вернёт true
array.map - вызывает функцию для каждого элемента массива и возвращает массив результатов выполнения этой функции
array.sort - сортирует массив на месте
array.reverse - меняет порядо на обратный
array.split(delim) - разбивает строку на массив по заданному разделителю delim, второй аргумент ограничивает кол-во эл-тов в массиве
array.join(glue) делает в точности противоположное split. Он создаёт строку из элементов array, вставляя glue между ними.
array.reduce - перебирем массив
Array.isArray(array) - работает как typeof
```
## Map
``` bash
new Map() – создаёт коллекцию.
map.set(key, value) – записывает по ключу key значение value.
map.get(key) – возвращает значение по ключу или undefined, если ключ key отсутствует.
map.has(key) – возвращает true, если ключ key присутствует в коллекции, иначе false.
map.delete(key) – удаляет элемент по ключу key.
map.clear() – очищает коллекцию от всех элементов.
map.size – возвращает текущее количество элементов.
map.keys() – возвращает итерируемый объект по ключам,
map.values() – возвращает итерируемый объект по значениям,
map.entries() – возвращает итерируемый объект по парам вида [ключ, значение], этот вариант используется по умолчанию в for..of.
```
## Set
``` bash
new Set(iterable) – создаёт Set, и если в качестве аргумента был предоставлен итерируемый объект (обычно это массив), то копирует его значения в новый Set.
set.add(value) – добавляет значение (если оно уже есть, то ничего не делает), возвращает тот же объект set.
set.delete(value) – удаляет значение, возвращает true, если value было в множестве на момент вызова, иначе false.
set.has(value) – возвращает true, если значение присутствует в множестве, иначе false.
set.clear() – удаляет все имеющиеся значения.
set.size – возвращает количество элементов в множестве.
```
