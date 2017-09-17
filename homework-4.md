## Домашняя работа №4
```
- В базе данных должны появиться таблицы с новостями и с авторами новостей. 
  Состав таблиц продумайте сами.
- В приложении - модели "Новость", "Автор" и связи между ними
- Предыдущее ДЗ в той части, которая про новости, перепишите, используя ORM
```

**Laravel**
* Созданы миграции для таблиц: [Авторы](https://github.com/skiphog/profit-laravel/blob/master/database/migrations/2017_09_17_152400_create_authors_table.php) и [Новости](https://github.com/skiphog/profit-laravel/blob/master/database/migrations/2017_09_17_152443_create_news_table.php)
* Связь Авторов - [один ко многим](https://github.com/skiphog/profit-laravel/blob/master/app/Author.php#L21). У новостей [обратная связь](https://github.com/skiphog/profit-laravel/blob/master/app/Article.php#L25).
* [Вывод новостей в шаблоне](https://github.com/skiphog/profit-laravel/blob/master/resources/views/news.blade.php) с переданной [коллекцией](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/NewsController.php).  

**Yii**

**Symfony**
