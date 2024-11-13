# kittygram

**Сервис для размещения своих любимых котиков.**

# Стэк

-Django

-Django-rest-framework

#Функционал

- Котики.

        Вы можете добавлять ваших котиков на всеобщее осмотрение. Так же не переживайте если вы выложили неудачную фотку ее всегда можно отредактировать. Так же вы можете поделиться выдающимися достижениями котиков.
  

# Запуск проекта.

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram_backend.git
```

```
cd kittygram_backend
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

* Если у вас Linux/macOS

    ```
    source env/bin/activate
    ```

* Если у вас windows

    ```
    source env/scripts/activate
    ```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Измените .env backend/ и опишите нужные вам данные в зависимости от ваших нужд.

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

Разместить ваш проект через докер: Измените файл .env.example в соответсвии с вашими данными так же обратите внимание на пункты DOCKER_USERNAME и DOCKER_PASSWORD.
```
docker compose up
```

# Пример работы

Все конечные точки и примеры входных и выходных данных доступны по url http://.../redoc/.


#Авторы

Носков Никита 

GitHub: 
https://github.com/NikitaNoscov
