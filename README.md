# Проект Foodgram
Адрес проекта: http://kittyfinal.hopto.org/
Администратор: test@test.ru
Пароль: test

# Foodgram реализован для публикации рецептов. Авторизованные пользователи могут подписываться на понравившихся авторов, добавлять рецепты в избранное, в покупки, скачать список покупок ингредиентов для добавленных в покупки рецептов.

API Документация http://kittyfinal.hopto.org/api/

В документации описаны возможные запросы к API и структура ожидаемых ответов. Для каждого запроса указаны уровни прав доступа.

# Технологии:
Python, Django, Django Rest Framework, Docker, Gunicorn, NGINX, PostgreSQL, Yandex Cloud, Continuous Integration, Continuous Deployment

# Запуск проекта на локальной машине:

Клонировать репозиторий:

https://github.com/iceeleoo/foodgram-project-react.git

В директории infra создать файл .env и заполнить своими данными по аналогии с example.env:

DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
DB_HOST=db
DB_PORT=5432
SECRET_KEY='секретный ключ Django'

Создать и запустить контейнеры Docker 

docker-compose -f docker-compose-local.yml up -d (использовать файл docker-compose с локальными настройками)

Создать и запустить контейнеры Docker, последовательно выполнить команды по созданию миграций, сбору статики, созданию суперпользователя.

После запуска проект будут доступен по адресу: http://localhost/

Документация будет доступна по адресу: http://localhost/api/docs/