## Домашняя работа №2
```
- Добавьте к своему проекту на Laravel middleware, реализующий следующую логику:
   ЕСЛИ в запросе от клиента присутствует заголовок X-UserName И значение этого заголовка "admin"
   ТО проверить наличие заголовка X-Password 
   И ЕСЛИ в нём содержится хэш пароля "123456"
   ТО продолжить работу
   ИНАЧЕ выдать статус 401 и прекратить обработку запроса
  
- Реализуйте аналогичную логику на двух других фреймворках  
```

**Laravel**
* [Реализация Middleware](https://github.com/skiphog/profit-laravel/blob/master/app/Http/Middleware/VerifyAuthentication.php)

**Yii**
* [Переопределил метод behaviors()](https://github.com/skiphog/profit-yii2/blob/master/controllers/TestVerifyController.php)
* [Фильтр](https://github.com/skiphog/profit-yii2/blob/master/components/Verify.php)

**Symfony**

В symfony нет Middleware как в Laravel и нет подобного механизма как в Yii.
Но в документации написано, что у symfony есть хороший способ вмешаться в Request, используя EventDispatcher component.
([Ссылка на документацию](http://symfony.com/doc/current/event_dispatcher/before_after_filters.html)). Я так и сделал.
* [Создал Event Subscriber](https://github.com/skiphog/profit-symfony/blob/master/src/AppBundle/EventSubscriber/TokenSubscriber.php) и реализовал заданную логику в нем. 




