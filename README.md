api_final
api final yatube

Описание.
Данный проект представляет собой API учебного проекта социальной сети Yatube. Здесь пользователи могут размещать свои публикации, создавать комментарии, подписываться на представляющих интерес авторов, либо отписываться при желании.

Технологии
Pythoт, Django, DRF, JWT + Djoser

Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/mariao-max/api_final_yatube
```

```
cd yatube_api
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source venv/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate

```

Создаем суперпользователя:


```
$ python manage.py createsuperuser
```

Запустить проект:

```
python manage.py runserver
```


