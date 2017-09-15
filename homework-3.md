## Домашняя работа №3
```
- Выведите в подвале главной страницы текущую дату
- Выведите 5 последних новостей, в каждой из которых могут быть заголовок, подзаголовок, 
  текст и изображения (передайте просто массив с этими новостями, не стоит делать модели и использовать БД)
- Добавьте форму для поиска по сайту, причем форма должна предлагать подсказки по мере ввода слов в строку поиска.

* Превратите вывод новостей из пункта 2 в Yii в виджет
```

**Laravel**
* [Вывод текущей даты](https://github.com/skiphog/profit-laravel/blob/master/resources/views/layouts/app.blade.php#L22)
* [Вывод новостей](https://github.com/skiphog/profit-laravel/blob/master/resources/views/testNews.blade.php) с [переданным массивом](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/TestNews.php)
* [Форма поиска](https://github.com/skiphog/profit-laravel/blob/master/resources/views/layouts/app.blade.php#L14) (Подключение библиотеки _select2_ в этом же файле)

**Yii**
* [Вывод текущей даты](https://github.com/skiphog/profit-yii2/blob/master/views/layouts/app.php#L34)
* [Форма поиска](https://github.com/skiphog/profit-yii2/blob/master/views/layouts/app.php#L26) (Подключение [библиотеки _Select2_ в Asset](https://github.com/skiphog/profit-yii2/blob/master/assets/AppAsset.php))
* [Виджет новостей](https://github.com/skiphog/profit-yii2/blob/master/components/NewsWidget.php) и [применение](https://github.com/skiphog/profit-yii2/blob/master/views/test-news/testNews.php)

**Symfony**
* [Вывод текущей даты](https://github.com/skiphog/profit-symfony/blob/master/app/Resources/views/base.html.twig#L24)
* [Вывод новостей](https://github.com/skiphog/profit-symfony/blob/master/app/Resources/views/default/test-news.html.twig) с [переданным массивом](https://github.com/skiphog/profit-symfony/blob/master/src/AppBundle/Controller/DefaultController.php#L27)
* [Форма поиска](https://github.com/skiphog/profit-symfony/blob/master/app/Resources/views/base.html.twig#L16) (Подключение библиотеки _select2_ в этом же файле)