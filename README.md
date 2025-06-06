# Kittygram
 ## Описание проекта
 Kittygram - сообщество любителей кошек, где каждый может похвастаться своим любимым питомцем.

 ## Функционал
 * Регистрация пользователя
 * Возможность добавлять фотографии котика, его дату рождения, цвет и список достижений

## Содержимое
* [Локальный запуск](#локальный-запуск)
* [Технологии](#технологии)
* [Автор](#автор)


## Локальный запуск:
```
docker compose up -d
docker compose exec backend python manage.py migrate
docker compose exec backend python manage.py collectstatic
docker compose exec backend cp -r /app/collected_static/. /backend_static/static/
```

Проект доступен по адресу:

```
http://127.0.0.1:9000/
```

## Технологии:
- Python
- Django Rest Framework
- PostgreSQL
- Nginx
- Docker

## Автор
* [Мехаев Александр](https://github.com/sashamehaev) alexandrmekhaev@yandex.ru