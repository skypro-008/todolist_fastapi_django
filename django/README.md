## Шаги:

### Установка

```console
pip install Django
django-admin startproject todoapp
```

### Запуск

```console
python manage.py migrate
python manage.py runserver
python manage.py startapp todolist
```

- добавьте 'todolist' в INSTALLED_APPS

### Добавление представлений
- реализуйте todolist.views.py и создайте todolist.urls.py
- добавьте urls в todoapp.urls.py

### Добавление шаблонов
- создайте папку templates и файл шаблона
- добавьте "templates" в DIR в settings.py
- измените представление: return render...

### Добавление моделей
- реализуйте todolist.models.py

### Сборка
```console
manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
```

- Добавление моделей на сайт админки:
    - todolist.admin.py: admin.site.register(Todo)
- войдите в админку

### добавление шаблона
- добавить {% csrf_token %} в шаблон

### CRUD
- реализуйте представления