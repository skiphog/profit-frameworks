## Домашняя работа №2
```
- Выведите в подвале главной страницы текущую дату
- Выведите 5 последних новостей, в каждой из которых могут быть заголовок, подзаголовок, 
  текст и изображения (передайте просто массив с этими новостями, не стоит делать модели и использовать БД)
- Добавьте форму для поиска по сайту, причем форма должна предлагать подсказки по мере ввода слов в строку поиска.

* Превратите вывод новостей из пункта 2 в Yii в виджет
```

**Laravel**
* [Текущая дата](https://github.com/skiphog/profit-laravel/blob/master/resources/views/layouts/app.blade.php#L22)
* [Новости](https://github.com/skiphog/profit-laravel/blob/master/resources/views/testNews.blade.php) с [переданным массивом](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/TestNews.php)
* [Форма поиска](https://github.com/skiphog/profit-laravel/blob/master/resources/views/layouts/app.blade.php#L14) (Подключение библиотеки в этом же файле)