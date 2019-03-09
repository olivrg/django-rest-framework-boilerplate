## Django Rest API Boilerplate

A simple REST API boilerplate with custom User model and token authentication. Tested and built with Django 2.1.7 and Django REST Framework.

## Project Structure

---

```sh
. django-rest-framework-boilerplate
├── app
│   ├── config
│   │   │── __init__.py
│   │   │── settings.py
│   │   │── urls.py
│   │   └── wsgi.py
│   ├── users
│   │   │── management
│   │   │   │── commands
│   │   │   │  │── __init__.py
│   │   │   │  └── wait_for_db.py
│   │   │   └── __init__.py
│   │   │
│   │   │── migrations
│   │   │   └── __init__.py
│   │   │
│   │   │── tests
│   │   │   │── __init__.py
│   │   │   │── test_admin.py
│   │   │   │── test_commands.py
│   │   │   │── test_models.py
│   │   │   └── test_users_api.py
│   │   │
│   │   │── __init__.py
│   │   │── admin.py
│   │   │── apps.py
│   │   │── models.py
│   │   │── serializers.py
│   │   │── urls.py
│   │   └── views.py
│   │
│   ├── .flake8
│   ├── db.sqlite3
│   └── manage.py
├── .gitignore
├── README.md
├── requirements.txt

```

### Installation

Cloning the repository in your virtualenv:

    $ git clone https://github.com/olivrg/django-rest-framework-boilerplate.git

    $ cd django-rest-framework-boilerplate

Install dependancies:

    $ pip install -r requirements.txt

Make migrations & migrate

    $ python manage.py makemigrations && python manage.py migrate

Create super user

    $ python manage.py createsuperuser

### Launching the app

    $ python manage.py runserver

### Create a new user

    Go to: http://127.0.0.1:8000/api/user/create/

### Run Tests

    $ python manage.py test

### Contributing

Contributions, questions and comments are welcome and encouraged.

## License

[MIT License](http://opensource.org/licenses/MIT).
