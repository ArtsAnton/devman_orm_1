# Урок №1 и №2  курса [Знакомство с Django: ORM](https://dvmn.org/modules/django-orm/)

Учебный проект, моделирующий систему контроля доступа к хранилющу.

Полезные ссылки:

* [PostgreSQL database adapter](https://pypi.org/project/psycopg2/);
* [Django web framework](https://www.djangoproject.com/);
* [Python-dotenv](https://pypi.org/project/python-dotenv/)

Начало работы:
1. Подготовка к работе;

```
pip install virtualenv
virtualenv -p /usr/bin/python3.6 venv
source venv/bin/activate
pip install -r requirements.txt 
```
2. Запуск проекта;
```
python manage.py runserver 0.0.0.0:8000
```

3. Перейдите на сайт по адресу [http://0.0.0.0:8000/](http://0.0.0.0:8000/) и проверьте его работу.

### Цель проекта

Код написан в образовательных целях в рамках выполнения урока № 1, №2 онлайн-курса для веб-разработчиков [devmn.org](https://dvmn.org/modules/django-orm/).
