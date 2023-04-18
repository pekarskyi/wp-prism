# wp-prism
Подключение Prism в WordPress. Syntax Highlighting: PHP, HTML, CSS, JS, C and other.<br>
Скрипт согласно функции работает только на страницах записей с тегом code.

## Подключение:
1.Загрузить папку в корень дочерней темы.<br>
2.Вставить функцию.

## Использование:
1.Вставить на страницу блок Код.<br>
2.Вставить сам код.<br>
3.Указать для записи тег code.<br>
4.В параметрах блока - Дополнительно - Дополнительные классы CSS указываем язык кода. Например: language-html, language-css, language-php или language-js.

## Примечание
В функции вместо проверки на наличие тега: 

```php
has_tag('code')
```
можно сделать проверку на произвольное поле (ACF). Например:

```php
get_field('code_enable')
```

Тип поля: Да/Нет<br>
Условия отображения: = запись<br>

Если в записи присутствует сниппет кода, то тогда не забываем отмечать чекбокс.

[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://sitex.me/standwithukraine)
