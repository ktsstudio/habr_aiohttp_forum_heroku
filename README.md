# Запуск

````
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python main.py
````

Сервер будет доступен по адресу http://0.0.0.0:8080/


# Публикация на Heroku

````
heroku login
heroku create
heroku addons:create heroku-postgresql:hobby-dev
heroku container:login
heroku container:push web
heroku container:release web
heroku open
````