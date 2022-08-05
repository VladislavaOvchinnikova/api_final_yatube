### YATUBE_API:
#### REST API для социальной сети Yatube, созданной в рамках курса [Python-разработчик от Яндекс.Практикум](https://practicum.yandex.ru/backend-developer/).

- [x] Позволяет делать запросы к моделям проекта: посты, группы, комментарии, подписки.

- [x] Поддерживает методы GET, POST, PUT, PATCH, DELETE.

- [x] Предоставляет данные в формате JSON.

#### Технологии
- Python 3.7
- Django==2.2.16
- djangorestframework==3.12.4
- djangorestframework-simplejwt==4.7.2

#### Как запустить проект
Клонировать репозиторий и перейти в него в командной строке:

```git clone https://github.com/VladislavaOvchinnikova/api_final_yatube.git```

```cd api_final_yatube```

Cоздать и активировать виртуальное окружение:

```python -m venv venv```

```source venv/Scripts/activate```

Установить зависимости из файла requirements.txt:

```python -m pip install --upgrade pip```

```pip install -r requirements.txt```

Выполнить миграции:

```python manage.py migrate```

Запустить проект:

```python manage.py runserver```
