### Задание №1
##### Ответ на HTML
```html
<form>
  <select>
    <option>
      1
    </option>
    <option>
      1
    </option>
  </select>
</form>
```
##### Ответ на Pug(Jade)
```jade
form
  select
    option 1
    option 2
```
### Задание №2
##### Ответ на HTML + CSS
```html
<ul>
    <li>
    1
    </li>
    <li>
    2
    </li>
</ul>
```
```css
li{
  list-style: none;
}

li:before{
  content: '+';
}
```
##### Ответ на Pug + Stylus
```jade
ul
  li 1
  li 2
```
```stylus
li
  list-style none

li:before 
  content '+'
```
### Задание №3
```css
display

position

float

z-index

top, right, bottom, left
```
### Задание №4 
#### jquery + ajax
```html
<body>
    <button id="but">Отправить запрос</button>
</body>
```
```javascript
$(document).ready(function(){
  $('#but').click(function(){
      $.ajax({
        type: 'GET',
        url: 'https://new-goga-pizza.herokuapp.com/api/en/pizza',
        success: function(res){
            console.log(res)
        }
      })
  });
});
```
#### Vue + axios
```vue
<template>
    <button @click="get">Отправить запрос</button>
</template>
<script>

export default {
    methods:{
        get(){
            axios.GET('https://new-goga-pizza.herokuapp.com/api/en/pizza').then(res=>{
                console.log(res)
            })
        }
    }
}
</script>
```
### Задание №5
```javascript
var x = {'a': 1, 'b':2, 'c':3}
console.log(Object.keys(x))
```
### Задание №6
```text 
Promise нужня для выполнения какой либо функции после получения результата из другой или даже нескольких функций
До Promise были Callback
В ES7 появился Observables
```

