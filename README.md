#  Django Mini Shop

Учебный интернет-магазин на Django с корзиной, авторизацией и подключением PostgreSQL.

---

##  Функционал

-  Просмотр списка товаров
-  Добавление товаров в корзину
-  Увеличение количества товаров
-  Очистка корзины
-  Авторизация пользователей
-  Ограничение: только авторизованные могут добавлять в корзину
-  Современный UI (карточки товаров, navbar, стили)

---

##  Технологии

- Python 3
- Django
- PostgreSQL
- HTML / CSS

---

##  Структура проекта
shop_for_students/
│
├── store/ # Основное приложение
├── static/
│ └── style/
│ ├── main.css
│ └── cart.css
├── media/ # Изображения товаров
├── templates/
├── manage.py

Настройка PostgreSQL

В student_shop/settings.py:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'student_shop',
        'USER': 'postgres',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
Перед запуском:

Создать базу данных student_shop
Выполнить миграции:
python manage.py migrate

Запуск проекта
python manage.py runserver

Открыть в браузере:

http://127.0.0.1:8000/

Админ-панель
http://127.0.0.1:8000/admin/

Создание администратора:

python manage.py createsuperuser

Возможные улучшения
 Удаление отдельного товара
 Кнопки + / -
 Оформление заказа
 Уведомления "товар добавлен"
 REST API (Django REST Framework)
