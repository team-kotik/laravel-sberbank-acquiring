# laravel-sberbank-acquiring
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)

Пакет предоставляет вашему приложению функциональность для работы с платежами с использованием эквайринга от Сбербанка.
Возможности:
- Создание и хранение платежей
- Логирование операций по платежам

Перед использованием рекомендуется ознакомиться с документацией, предоставляемой Сбербанком.

## Требования
* PHP >= 8.0
* Laravel >= 7.0
* Расширения PHP: ext-json, ext-curl
* Реляционная БД

## Установка
Добавьте пакет в зависимости:
```
composer require team-kotik/laravel-sberbank-acquiring
```

Опубликуйте файл настроек:
```
php artisan vendor:publish --provider="Aleksandr\SberbankAcquiring\Providers\AcquiringServiceProvider" --tag=config
```

Опубликуйте файлы миграций:
```
php artisan vendor:publish --provider="Aleksandr\SberbankAcquiring\Providers\AcquiringServiceProvider" --tag=migrations
```

Запустите миграции:
```
php artisan migrate
```

## Лицензия (License)
The MIT License (MIT). Please see [License File](https://github.com/team-kotik/laravel-sberbank-acquiring/blob/main/LICENSE) for more information.
