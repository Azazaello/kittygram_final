<<<<<<< HEAD
=======
# Kittygram 

## Описание проекта:
Kittygram - это платформа для обмена фотографиями кошек, созданная с использованием Django и React. На ней пользователи могут выкладывать, просматривать и изменять посты с подробностями о кошках.

## Технологии:

Python  
Django  
React  
Nginx  
Gunicorn  
Certbot
Docker 
Github Actions

## Инструкция по запуску:

### Клонируйте репозиторий:   
```sh/bash
git@github.com:AliceBolgarina/.git
```
   
```sh/bash
cd kittygram
```
Выполнить запуск:

```sh/bash
sudo docker compose -f docker-compose.yml up
```

Выполнить миграции и сбор статики: 

```sh/bash
sudo docker compose -f docker-compose.yml exec backend python manage.py migrate
sudo docker compose -f -docker-compose.yml exec backend python manage.py collectstatic --no-input
sudo docker compose -f docker-compose.yml exec backend cp -r /app/collected_static/. /static/static/
```

## Автор: 
   
[Азиза](https://github.com/Azazaello)
>>>>>>> origin/main
