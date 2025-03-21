# Проект API для Yatube
Проект в виде социальной сети с публикациями, комментариями, группами и подписками.

# Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/Vengerian/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python -m venv .venv
```

```
.venv/bin/activate
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

Запустить проект:

```
python manage.py runserver
```

# Примеры некоторых запросов:
- Публикация поста
```
POST /api/v1/posts/
{
    "text": "string"
}
```
- Удаление комментария

```
DEL /api/v1/posts/{post_id}/comments/{comment_id}/
```
