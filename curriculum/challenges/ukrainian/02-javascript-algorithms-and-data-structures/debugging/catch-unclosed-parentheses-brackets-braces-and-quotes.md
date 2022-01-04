---
id: 587d7b84367417b2b2512b36
title: 'Знаходження незакритих круглих, квадратних і фігурних дужок та лапок'
challengeType: 1
forumTopicId: 301190
dashedName: catch-unclosed-parentheses-brackets-braces-and-quotes
---

# --description--

Наступна синтаксична помилка, про яку варто пам'ятати - відкривши круглі, квадратні, фігурні дужки або лапки, необхідно їх також закрити. Зазвичай про це можна забути під час редагування вже існуючого коду або вставлення елементів вже з одним з типів парних розділових знаків. Також будьте обережні, коли вкладаєте одні блоки коду в інші, наприклад, додавання зворотного виклику функції в якості аргументу до методу.

Один із способів уникнути цієї помилки - одразу при відкритті лапок або дужок закривайте їх і потім повертайте курсор між парними пунктуаційними знаками та продовжуйте кодування. На щастя, більшість сучасних редакторів коду створюють другу частину пари автоматично.

# --instructions--

Виправте помилки парних знаків у коді.

# --hints--

Ваш код має виправити відсутній фрагмент масиву.

```js
assert(code.match(/myArray\s*?=\s*?\[\s*?1\s*?,\s*?2\s*?,\s*?3\s*?\];/g));
```

Ваш код має виправити відсутній фрагмент методу `.reduce()`. Вихідні дані консолі повинні мати результат `Sum of array values is: 6`.

```js
assert(arraySum === 6);
```

# --seed--

## --seed-contents--

```js
let myArray = [1, 2, 3;
let arraySum = myArray.reduce((previous, current =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
```

# --solutions--

```js
let myArray = [1, 2, 3];
let arraySum = myArray.reduce((previous, current) =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
```