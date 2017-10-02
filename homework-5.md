## Домашняя работа №5
**	Работа с базой данных. Слой ORM.**
```
Сделайте в вашем приложении базу данных, которая отражает следующие сущности:
  - Новости: с заголовками, текстом, датой публикации, датой модификации, рубрикой, признаком 
    "списано в архив"
  - Рубрики новостей
  
Решите в каждом из фреймворков следующие задачи, используя возможности ORM этих фреймворков:
  - Получение списка "неархивных" новостей за текущую неделю, в разбивке по дням недели и по рубрикам.
  - Отображение этого списка на странице сайта, причем если новость редактировалась после публикации - 
    должна стоять метка "Обновлено".
  - Списание в архив всех новостей из выбранных рубрик, которые были опубликованы ранее указанной даты.
```

**Laravel**
 * Миграции для [новостей](https://github.com/skiphog/profit-laravel/blob/master/database/migrations/2017_09_17_152443_create_news_table.php) и [рубрик](https://github.com/skiphog/profit-laravel/blob/master/database/migrations/2017_09_17_152442_create_rubrics_table.php)
 * [Получение списка](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/NewsController.php#L23) "неархивных" новостей за текущую неделю, в разбивке по дням недели и по рубрикам. [С помощью метода в модели.](https://github.com/skiphog/profit-laravel/blob/master/app/Article.php#L65)
 * [Отображение этого списка на странице сайта](https://github.com/skiphog/profit-laravel/blob/master/resources/views/newsByRubrics.blade.php#L29), причем если новость редактировалась после публикации - должна стоять метка "Обновлено".
 * [Списание в архив всех новостей](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/NewsController.php#L36) из выбранных рубрик, которые были опубликованы ранее указанной даты.
