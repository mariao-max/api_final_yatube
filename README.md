#  api final yatube

## Описание
Данный проект представляет собой API учебного проекта социальной сети Yatube. Здесь пользователи могут размещать свои публикации, создавать комментарии, подписываться на представляющих интерес авторов, либо отписываться при желании.

## Технологии
Pythoт, Django, DRF, JWT + Djoser

## Установка

* Клонировать репозиторий

 > git clone https://github.com/mariao-max/api_final_yatube <br/>

* Перейти в директорию проекта

> cd yatube_api 

* Cоздать и активировать виртуальное окружение:

> python -m venv env

> source venv/Scripts/activate

* Установить зависимости из файла requirements.txt:

> python -m pip install --upgrade pip

> pip install -r requirements.txt

* Выполнить миграции:

> python manage.py migrate

* Создать суперпользователя:

> python manage.py createsuperuser

* Запустить проект:

> python manage.py runserver

## Примеры запросов и ответов
* Пример GET-запроса <br/>
http://127.0.0.1:8000/api/v1/posts/
* Ответ на GET-запрос <br/>
{ <br/>
        "id": 2, <br/>
        "author": "odrin", <br/>
        "text": "Мы только оттого мучаемся прошедшим и портим себе будущее, что мало заняты настоящим. Прошедшее было, будущего нет, есть только одно настоящее.", <br/>
        "pub_date": "2022-02-02T09:01:46.789732Z", <br/>
        "image": null, <br/>
        "group": 2 <br/>
 } <br/>

* Пример POST-запроса для авторизованного пользователя (с использванием токена) <br/>
http://127.0.0.1:8000/api/v1/posts/ <br/>
Authorization: Bearer Токен <br/>
{ <br/>
    "text": "Пример POST запроса" <br/>
} <br/>
* Ответ на POST-запрос: <br/>
{ <br/>
    "id": 3, <br/>
    "author": "odrin", <br/>
    "text": "Пример POST запроса", <br/>
    "pub_date": "2022-02-03T12:04:13.417756Z", <br/>
    "image": null, <br/>
    "group": null <br/>
<<<<<<< HEAD
} <br/>
=======
} <br/>
>>>>>>> 0dafe261ab2288fc13d069e95a18e7f7c5b23b91
