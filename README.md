# Урок №1 и №2  курса [Знакомство с Django: ORM](https://dvmn.org/modules/django-orm/)

Учебный проект, моделирующий систему контроля доступа к хранилющу.

Полезные ссылки:

* [PostgreSQL database adapter](https://pypi.org/project/psycopg2/);
* [Django web framework](https://www.djangoproject.com/);
* [Python-dotenv](https://pypi.org/project/python-dotenv/);
* [Environs](https://pypi.org/project/environs/).

Начало работы:
1. Подготовка к работе;

```
pip install virtualenv
virtualenv -p /usr/bin/python3.6 venv
source venv/bin/activate
pip install -r requirements.txt 
```

2. Создаем файл .env со следующим содержимым:

```
# Настройка БД
DB_ENGINE=django.db.backends.postgresql_psycopg2
DB_HOST=checkpoint.devman.org
DB_PORT=5434
DB_NAME=checkpoint
DB_USER_PASSWORD=your_password
DB_USER=your_user

# Секретный ключ
SECRET_KEY=your_key

# Режим работы
DEBUG=False

# Список хостов доступных для работы (в данном случае только локально). 
ALLOWED_HOSTS=localhost,127.0.0.1
```

Данные переменные используются для настройки - [settings.py](https://github.com/ArtsAnton/devman_orm_1/blob/main/project/settings.py).

3. Запуск проекта;
```
python manage.py runserver localhost:8000
```

3. Перейдите на сайт по адресу [http://localhost:8000/](http://localhost:8000/) и проверьте его работу.

### Цель проекта

Код написан в образовательных целях в рамках выполнения урока № 1, №2 онлайн-курса для веб-разработчиков [devmn.org](https://dvmn.org/modules/django-orm/).
