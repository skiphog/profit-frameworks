## Домашняя работа №5
**Работа с базой данных. Слой ORM.**
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
 * Миграции для [новостей и рубрик](https://github.com/skiphog/profit-laravel/tree/master/database/migrations)
 * [Получение списка](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/NewsController.php#L23) "неархивных" новостей за текущую неделю, в разбивке по дням недели и по рубрикам. [С помощью метода в модели.](https://github.com/skiphog/profit-laravel/blob/master/app/Article.php#L65)
 * [Отображение этого списка на странице сайта](https://github.com/skiphog/profit-laravel/blob/master/resources/views/newsByRubrics.blade.php#L29), причем если новость редактировалась после публикации - должна стоять метка "Обновлено".
 * [Списание в архив всех новостей](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Controllers/NewsController.php#L36) из выбранных рубрик, которые были опубликованы ранее указанной даты.
 
 **Yii2**
 * Миграции для [новостей и рубрик](https://github.com/skiphog/profit-yii2/tree/master/migrations)
 * [Получение списка](https://github.com/skiphog/profit-yii2/blob/master/controllers/NewsController.php#L22) "неархивных" новостей за текущую неделю, в разбивке по дням недели и по рубрикам. [С помощью метода в модели.](https://github.com/skiphog/profit-yii2/blob/master/models/Article.php#L60)
 * [Отображение этого списка на странице сайта](https://github.com/skiphog/profit-yii2/blob/master/views/news/newsByRubrics.php#L30), причем если новость редактировалась после публикации - должна стоять метка "Обновлено".
 * [Списание в архив всех новостей](https://github.com/skiphog/profit-yii2/blob/master/controllers/NewsController.php#L32) из выбранных рубрик, которые были опубликованы ранее указанной даты.
 