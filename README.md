# API Сервис заказа товаров для розничных сетей.
**Masagutov Radik**

## Описание

Приложение предназначено для автоматизации закупок в розничной сети. Пользователи сервиса — покупатель (менеджер торговой сети, который закупает товары для продажи в магазине) и поставщик товаров.

**Клиент (покупатель):**

- Менеджер закупок через API делает ежедневные закупки по каталогу, в котором
  представлены товары от нескольких поставщиков.
- В одном заказе можно указать товары от разных поставщиков — это
  повлияет на стоимость доставки.
- Пользователь может авторизироваться, регистрироваться и восстанавливать пароль через API.
    
**Поставщик:**

- Через API информирует сервис об обновлении прайса.
- Может включать и отключать прием заказов.
- Может получать список оформленных заказов (с товарами из его прайса).


**Технологии в проекте:**
* Рython 3;
* Django;
* Django Rest Framework;
* Postgresql;
* Postman
* Celery;
* Redis server;
* Docker;
* Docker-compose.

## Запуск проекта

1. Склонировать репозиторий при помощи git:
```bash
git clone https://github.com/radik121/python-final-diplom.git
```

2. Перейти в корневую папку проекта:
```bash
cd python-final-diplom
```

3. Для запуска проекта выполнить команду:
```bash
docker-compose up -d
```

4. Для создания суперпользователя ввести команду:
```bash
docker-compose exec -it api python manage.py createsuperuser
```

**Приложение доступно по адресу:** http://127.0.0.1:8000

**API запросы доступны на сервере POSTMAN:** https://documenter.getpostman.com/view/22128489/UzXNTwjw

