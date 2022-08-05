### YATUBE_API:
#### REST API для социальной сети Yatube, созданной в рамках курса [Python-разработчик от Яндекс.Практикум](https://practicum.yandex.ru/backend-developer/).

- [x] Позволяет делать запросы к моделям проекта: посты, группы, комментарии, подписки.

- [x] Поддерживает методы GET, POST, PUT, PATCH, DELETE.

- [x] Предоставляет данные в формате JSON.

#### Технологии
- Python 3.2
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

#### Примеры запросов

##### POSTS / Посты

```api/v1/posts/``` (GET, POST) - получить список всех постов или создать новый пост.

```api/v1/posts/{post_id}/``` (GET, PUT, PATCH, DELETE) - получить, обновить, частично обновить или удалить конкретный пост.

##### COMMENTS / Комментарии

```api/v1/posts/{post_id}/comments/``` (GET, POST) - получить список всех комментариев к посту или создать новый комментарий.

```api/v1/posts/{post_id}/comments/{comment_id}/``` (GET, PUT, PATCH, DELETE) - получить, обновить, частично обновить или удалить конкретный комментарий.

##### GROUPS / Группы

```api/v1/groups/``` (GET, POST) - получить список всех групп или создать новую группу.

##### FOLLOW/ Подписки

```api/v1/follow/``` (GET, POST) - получить список всех подписчиков или создать новую подписку.
