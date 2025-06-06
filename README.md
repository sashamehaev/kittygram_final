# Kittygram
 ## Описание проекта
 Kittygram - сообщество любителей кошек, где каждый может похвастаться своим любимым питомцем.

 ## Функционал
 * Регистрация пользователя
 * Просмотр котиков всех пользователей
 * При создании котика добавляются его фотографии, имя, цвет, год рождения и достижения

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

## Примеры запросов
 * При GET запросе будут отправлены все котики клиенту
 * При POST запросе будет создан котик
 ```
 https://sashamehaev-kittygr.bounceme.net/api/cats
 ```

 При запросе по этому адресу можно получить, отредактировать или удалить котика
 ```
 https://sashamehaev-kittygr.bounceme.net/api/cats/pk
 ```

 * При GET запросе будут отправлены все достижения клиенту
 * При POST запросе будет создано новое достижение
 ```
 https://sashamehaev-kittygr.bounceme.net/api/achievements
 ```

 При запросе по этому адресу можно получить, добавить, обновить, удалить достижения котика
 ```
 https://sashamehaev-kittygr.bounceme.net/api/achievements/pk
 ```

 Панель администратора
 ```
 https://sashamehaev-kittygr.bounceme.net/admin
 ```

## Технологии:
- Python
- Django Rest Framework
- PostgreSQL
- Nginx
- Docker

## Автор
* [Мехаев Александр](https://github.com/sashamehaev)
* Почта alexandrmekhaev@yandex.ru