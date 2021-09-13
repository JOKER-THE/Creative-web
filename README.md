Решение тестового задания для PHP-программиста
=====================================

Развертывание проекта
--------------

1. Склонируейте проект из репозитория `git clone git@github.com:JOKER-THE/Creative-web.git`
2. Из каталога необходимо распаковать composer-пакеты с помощью команды `composer install`
3. Для работы с докером используйте **Docker-compose.yaml**
4. Для локальной работы с Apache необходимо выполнить следующие шаги:
- Настроить обращение Apache к **index.php** в каталоге **public** 
- Создать документ **.env.local** с настройками окружения `APP_ENV=dev` и подключения к БД `DATABASE=mysql://username:password@localhost:3306/database`
- Создать документ **app.dev.yaml** в каталоге **config**, скопировав код из файла **app.yaml** в каталоге **config**
5. Обновите структуру БД с помощью команды `php ./bin/console orm:schema-tool:update`

Импорт данных из [iTunes Movie Trailers](https://trailers.apple.com)
--------------

Импорт выполняется с помощью консольной команды `php ./bin/console fetch:trailers`
