___
# МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ПРОФЕСИОНАЛЬНОГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»
### <p align="center">Лабораторная работа №6 “CSS”</p> 
#### <br><p align="right">Подготовил студент направления подготовки 01.03.02 «Прикладная математика и информатика»<br> Института естественных наук и техносферной безопасности<br> Зураев Дмитрий Бакенович.</p><br><p align="right">Научный руководитель:<br> Соболев Евгений Игоревич</p><br> <p align="center">Южно-Сахалинск 2023 г.</p>
___
### <p align="center">Введение</p>
<p align="justify">CSS (Cascading Style Sheets) является языком стилей, который используется для оформления и визуального представления веб-страниц. В этой лабораторной работе мы будем исследовать концепцию селекторов в CSS и создадим несколько страниц по шаблону. Также сделаем практические задания по css.</p>

### <p align="center">Цели</p>
<p align="justify">Изучить и практически применить различные типы и комбинации CSS селекторов для точного выбора и стилизации элементов на веб-странице, поработать с заданиями на JS.</p>

### <p align="center">Задачи</p>
<p align="justify">Применить технологию CSS и JS.</p>

____________________
## <p align="center">_Решение_</p>
1. Придумайте селектор, который выберет абзацы `<p>` внутри дивов `<div>`
```css
div p {}
```
2. Придумайте селектор, который выберет все `<h2>` внутри дивов `<div>`
```css
div h2 {}
```
3. Придумайте селектор, который выберет все абзацы `<p>` из элемента с `id=test`
```css
#test p {}
```
4. Придумайте селектор, который выберет все `<h2>` из элемента с `id=test`
```css
#test h2 {}
```
5. Выберите все элементы с классом `bbb`
```css
.bbb {}
```
6. Выберите все элементы с классом bbb из элемента с `id=test`
```css 
#test .bbb {}
```
7. Выберите все абзацы `<p>` с классом `bbb`
```css
p.bbb {}
```
8. Выберите все `<h2>` с классом `bbb`
```css
h2.bbb {}
```
9. Выберите все абзацы `<p>` с классом `bbb` из элемента с `id=test`
```css
#test p.bbb {}
```
10. Выберите все элементы с классом `bbb` и элементы с классом `xxx` одновременно
```css
.bbb, .xxx {}
```
11. Выберите все абзацы `<p>` с классом bbb и `<h2>` с классом `xxx` одновременно
```css
p.bbb, h2.xxx {}
```
12. Выберите все абзацы `<p>` с классом `bbb` из `id=test` и все абзацы `<p>` с классом `xxx` из `id=test` одновременно
```css
#test p.bbb, #test p.xxx {}
```
13. Выберите все элементы из класса `fff`
```css
.fff * {}
```
14. Выберите все абзацы `<p>` из класса `fff`
```css
.fff p {}
```
15. Выберите все абзацы `<p>` с классом `fff`
```css
p.fff {}
```
16. Выберите все элементы с классом `bbb` из класса `fff`
```css
.fff .bbb {}
```
17. Выберите все `<h2>` с классом bbb из класса `fff`
```css
.fff h2.bbb {}
```
18. Сделайте селектор, который выберет все ссылки из `id=test`, с состояния `link` и `visited` сделайте неподчеркнутыми и красными, а состояние `hover` - подчеркнутым и голубым
```css
#test a:link, #test a:visited {
  text-decoration: none; 
  color: red;
}
#test a:hover {
  text-decoration: underline; 
  color: blue; 
}
```
19. Сделайте селектор, который выберет все ссылки с классом `www`, состояния `link` и `visited` сделайте подчеркнутыми и голубыми, а состояние `hover` - неподчеркнутым.
```css
a.www:link, a.www:visited {
  text-decoration: underline; 
  color: blue; 
}
a.www:hover {
  text-decoration: none; 
}
```
20. Сделайте селектор, который выберет все ссылки из `id=test` с классом `www`. Цвета состояний выберите самостоятельно
```css
#test a.www{
    color: burlywood;
}
```
21. Сделайте селектор, который выберет все ссылки из `class=eee` с классом `www`. Цвета состояний выберите самостоятельно
```css
.eee a.www {
    color: turquoise;
}
```
[1]: 22.png
[2]: 23.png
[3]: 24.png
[4]: 25.png
[5]: 26.png
[6]: 27.png
22. Повторите страницу по данному по образцу: ![Задание22][1]
```css
.hello{
    border-color: gray;
    border-style: dotted;
    color: black;
}
#und{
    text-decoration: underline;
}
#lThr{
    text-decoration: line-through;
}
#over{
    text-decoration: overline;
}
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style22.css">
</head>
<body>
    
    <div class="hello">
        <p id="und">Привет, мир!</p>
        <p id="lThr">Привет, мир!</p>
        <p id="over">Привет, мир!</p>
    </div>
</body>
</html>
```
23. Повторите страницу по данному по образцу: ![Задание23][2]
```css
.hello{
    border-color: gray;
    border-style: dotted;
    color: black;
}
.red-square {
    width: 200px;
    height: 200px;
    border: 2px solid red;
    margin: 15px auto 15px 15px;
}
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style23.css">
</head>
<body>
    <div class="hello">
        <div class="red-square"></div>
    </div>
</body>
</html>
```
24. Повторите страницу по данному по образцу: ![Задание24][3]
```css
.hello{
    border-color: gray;
    border-style: dotted;
    color: black;
}
.square {
    width: 600px;
    height: 200px;
    border: 2px dotted blue;
    margin: 15px auto 15px 15px;
}
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style24.css">
</head>
<body>
    <div class="hello">
        <div class="square"></div>
    </div>
</body>
</html>
```
25. Повторите страницу по данному по образцу: ![Задание25][4]
```css
.hello{
    border-color: gray;
    border-style: dotted;
    color: black;
}
.square {
    width: 300px;
    height: 300px;
    border: 2px dotted green;
    border-radius: 10px 25px 10px 25px;
    margin: 15px auto 15px 15px;
}
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style25.css">
</head>
<body>
    <div class="hello">
        <div class="square"></div>
    </div>
</body>
</html>
```
26. Повторите страницу по данному по образцу: ![Задание26][5]
```css
.hello{
    border-color: gray;
    border-style: dotted;
    color: black;
}
.circle {
    width: 100px;
    height: 100px;
    border: 2px solid red;
    border-radius: 50%;
    margin: 15px auto 15px 15px;
}
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style26.css">
</head>
<body>
    <div class="hello">
        <div class="circle"></div>
    </div>
</body>
</html>
```
27. Повторите страницу по данному по образцу: ![Задание27][6]
```css
.hello{
    border-color: gray;
    border-style: dotted;
    color: black;
}
.ourLink {
    margin: 15px auto 15px 15px;
}
#firLink{
    color: green;
}
#secLink{
    color: red;
}
#thiLink{
    color: black;
    text-decoration: none; 
}
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style27.css">
</head>
<body>
    <div class="hello">
        <div class="ourLink">
            <a href="" id="firLink">ссылка</a><br><br>
            <a href="" id="secLink">ссылка</a><br><br>
            <a href="" id="thiLink">ссылка</a><br><br>
        </div>
    </div>
</body>
</html>
```
[Kata1](https://www.codewars.com/kata/555de49a04b7d1c13c00000e)
```javascript
function add(...numbs) {
    let sum = 0;
    for (let i = 1; i <= numbs.length; i++) {
        sum += numbs[i - 1] / i;
    }
    return Math.round(sum);
}
```
[Kata2](https://www.codewars.com/kata/588453ea56daa4af920000ca)
```javascript
function arrayPacking(a) {
return a.reduce(
    (value, byte, i) => value + byte * Math.pow(256, i)
  );
}
```
[Kata3](https://www.codewars.com/kata/55e9529cbdc3b29d8c000016)
```javascript
function charToAscii(string){
  if (string.length === 0) {
    return null;
  }
  let asciiHash = {};
  for (let i = 0; i < string.length; i++) {
    let char = string[i];
    if (!char.match(/[a-zA-Z]/)) {
      continue;
    }
    if (asciiHash[char]) {
      continue;
    }
    let asciiValue = char.charCodeAt(0);
    asciiHash[char] = asciiValue;
  }
  return asciiHash;
}
```
[Kata4](https://www.codewars.com/kata/55968ab32cf633c3f8000008)
```javascript
function initials(n){
  let initials = "";
  const names = n.split(" ");
  for (let i = 0; i < names.length; i++) {
    let name = names[i];
    if (i === names.length - 1) {
      initials += name.charAt(0).toUpperCase() + name.slice(1);
    } else {
      initials += name.charAt(0).toUpperCase() + ".";
    }
}
    return initials;
}
```
[Kata5](https://www.codewars.com/kata/55ee3ebff71e82a30000006a)
```javascript
function titleToNumber(title) {
  let columnNumber = 0;

  for (let i = 0; i < title.length; i++) {
    let char = title[i];
    let charNumber = char.charCodeAt(0) - 64;
    columnNumber = columnNumber * 26 + charNumber;
  }

  return columnNumber;
}
```
[Kata6](https://www.codewars.com/kata/5412509bd436bd33920011bc)
```javascript
function maskify(cc) {
  let ccChars = cc.split('');
  for (let i = 0; i < ccChars.length - 4; i++) {
    ccChars[i] = '#';
  }
  cc = ccChars.join('');
  return cc;
}
```
## <p align="center">_Вывод_</p>
Таким образом, я научился работать с селекторами в CSS, применять стили для отдельных тегов, классов и id на странице. Также поработал со строками в JS.
