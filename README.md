## Структура проекта

```
my_cat_site/
├── app.py
├── models.py
├── forms.py
├── requirements.txt
├── instance/
│   └── site.db
├── templates/
│   ├── base.html
│   ├── home.html
│   ├── about.html
│   ├── private.html
│   ├── login.html
│   ├── register.html
│   └── layout.html
├── static/
│   ├── css/
│   │   └── style.css
│   └── images/
│       ├── cat.jpg
│       └── cat2.jpg
```

## 1. Установка зависимостей

Создайте файл `requirements.txt`:
```
flask
flask-login
flask-wtf
flask-sqlalchemy
werkzeug
email-validator
```

Установите зависимости:
```bash
pip install -r requirements.txt
```

## Запуск приложения

1. Создайте базу данных:
```bash
flask shell
>>> from app import db
>>> db.create_all()
>>> exit()
```

2. Запустите приложение:
```bash
python app.py
```

![image](https://github.com/user-attachments/assets/51aef5c9-56c1-449d-a2a4-22d4b14606c4)

