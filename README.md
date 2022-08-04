# API для сервиса Yatube
### Описание:
API для соцсети Yatube представляет позволяет публиковать, редактировать и удалять посты, комментировать записи, редактировать и удалять свои комментарии, а также подписываться на авторов или отписываться от них.
### Технологии:
Python 3.7
Django 2.2.16
djangorestframework-simplejwt==4.7.2
### Установка проекта в dev-режиме:
- Клонируйте репозиторий на Ваш компьютер
- Создайте и активируйте виртуальное окружение
```
python -m venv venv

source venv/Scripts/activate
``` 
-  Установите все зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 
- Выполните миграции
```
python manage.py migrate
``` 
- Запустите сервер :
```
python manage.py runserver
```
### Примеры запросов к API:
```
/api/v1/posts/   (GET, POST, PUT, PATCH, DELETE)
/api/v1/posts/<id>   (GET, POST, PUT, PATCH, DELETE)
/api/v1/posts/<id>/comments  (GET, POST, PUT, PATCH, DELETE)
/api/v1/posts/<id>/comments/<id>  (GET, POST, PUT, PATCH, DELETE)
/api/v1/group/ (GET, POST)
/api/v1/follow/  (GET, POST)
```

### Автор:
Светлана Ременюк
