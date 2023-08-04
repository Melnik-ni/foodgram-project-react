# Продуктовый помощник Foodgram

Продуктовый помощник - дипломный проект курса Backend-разработки Яндекс.Практикум. Проект представляет собой онлайн-сервис и API для него. На этом сервисе пользователи смогут публиковать рецепты, подписываться на публикации других пользователей, добавлять понравившиеся рецепты в список «Избранное», а перед походом в магазин скачивать сводный список продуктов, необходимых для приготовления одного или нескольких выбранных блюд.

Проект реализован на `Django` и `DjangoRestFramework`. Доступ к данным реализован через API-интерфейс. Документация к API написана с использованием `Redoc`.

## Стек технологий:

* Python 3.7
* Django
* DRF
* Docker

## Как развернуть проект

1. Выполните команду:
- sudo docker-compose up -d --build
2. Выполните миграции:
- sudo docker-compose exec backend python manage.py makemigrations
- sudo docker-compose exec backend python manage.py migrate
3. Соберите статику:
- sudo docker-compose exec backend python manage.py collectstatic --no-input
4. Заполните базу ингредиентами:
- sudo docker-compose exec backend python manage.py load_data
5. Создайте суперюзера:
- sudo docker-compose exec backend python manage.py createsuperuser

**Для корректного создания рецепта через фронт, надо создать пару тегов в базе через админ зону.**


## Автор
[Ибраев Николай](https://github.com/Melnik-ni)

## Проект можно посмотреть по ссылке [Еда](http://158.160.28.251/recipes)


## СуперЮзер

Почта - qwerty@mail.ru
Пароль - A54535251
