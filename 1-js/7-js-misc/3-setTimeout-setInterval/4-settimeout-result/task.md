# Что выведет setTimeout?

[importance 5]

В коде ниже запланирован запуск `setTimeout`, а затем запущена тяжёлая функция `hardWork`, выполнение которой занимает более долгое время, чем интервал до срабатывания таймера. 

Когда сработает `setTimeout`? Выберите нужный вариант:
<ol>
<li>До выполнения `hardWork`.</li>
<li>Во время выполнения `hardWork`.</li>
<li>Сразу же по окончании `hardWork`.</li>
<li>Через 100мс после окончания `hardWork`.</li>
</ol>

Что выведет `alert` в коде ниже?

```js
setTimeout(function() {
  alert( i );
}, 100);

var i;

function hardWork() {
  // время выполнения этого кода >100мс, сам код неважен
  for (i = 0; i < 1e8; i++) hardWork[i % 2] = i;
}

hardWork();
```

