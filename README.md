# Первый взгляд на display:grid
Ух... Я это запилила... Хотя если бы не [Наталья Давыдова](https://github.com/nat-davydova), я так бы и облизывалась на display:grid

## Что не удалось
1. Раскачать `grid-auto-flow: dance;` Потому что я жестко контролю размеры, и этому "танцу" просто некуда встроиться. Т.е. нету дырок для впихивания... Пока не могу понять как это ТОЧНО работает.
2. Адекватно имитировать масонри. Именно потому что нет пп 1. Масонри требует ПЛОТНОЙ порядковой "застройки". dance ее не дает. Точнее дает, но не порядок. С этой точки `column-count` просто идеален. Как был, так и остается пока не будет реализовано `grid-template-*:  masonry;`, да и вообще `masonry` в гридах. Кроче, дастаем Ждунов и... Ждем.)
3. Выломать из грида потомка - это я вам доложу то еще занятие. 🤣
НО мне это удалось. И опять помог старый хак с отрицательным маргином.)))
И да, там есть баг со всплывающим описанием, который я не придумала (не сумела расчитать) как вернуть в "границы" контейнера. Математика меня имеет. Но это пока... 😈

## Из плюшек и фич
1. Удалось пощупать "беcконтейнерный" подход на `grid-area` и именованных линиях. Это КРУТО!!! НО опять же, контейнеры вам нужны, ибо без них никаких более сложных сеток окромя спостого свитка вы не построите.
И ДА! ТАК можно сделать секцию разрывающую контейнер. НО невозможно сделать сетку ВНУТРИ этой секции... Или я не знаю как...
2. Если нету/поломался/неподгрузился имидж - у вас ничего не умрет и не поедет. Это мы умеем.

В целом, все в коде.
Будут вопросы, найдены баги, будут рекомендации/предложения/советы или даже желание подтянуть меня по грид - я тут И тогов как ПионЭр!

## Дисклеймер
В ДАННОЙ ВЕРСТКЕ МНЕ ПРИНАДЛЕЖИТ ТОЛЬКО КОД. ВСЕ ДИЗАЙНЫ, ИЗОБРАЖЕНИЯ ПРИНАДЛЕЖАТ ИХ СОЗДАТЕЛЯМ. ОТКАЗЫВАЮСЬ ОТ ЛЮБЫХ ПРИТЯЗАНИЙ. БЛАГОДАРЮ ЗА ТАКИЕ СОЧНЫЕ И КРУТЫЕ РАБОТЫ, ОНИ РЕАЛЬНО ОЖИВИЛИ ВЕРСТКУ!
