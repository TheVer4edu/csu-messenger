# Курс "Разработка интернет-приложений"

## 1 задание

1. По аналогии с пользователями, реализовать crud методы для чатов. Все входные и выходные данные должны быть явно прописаны через Pydantic-схемы. При этом get запрос должен возвращать не только информацию о чате, но и список участников-пользователей
2. Продумать сущность "Сообщение", реализовать методы:
   - Отправка сообщения в чат
   - Редактирование сообщения
   - Удаление сообщения
   - Список из N последних сообщений в чате
   - Список из N чатов, в которых была последня активность

## 2 задание

- Работу с чатами аналогично перевести на работу с БД - добавить sqlalchemy-модели, миграции, переписать crud-методы

## Полезные команды

- Создание миграции
```
.\venv\Scripts\python.exe -m alembic revision --autogenerate -m "Поменяли password на hashed_password"
```

- Заполнение миграций
`.\venv\Scripts\python.exe -m alembic upgrade head`

- Запуск докер-контейнеров
`docker-compose up -d`