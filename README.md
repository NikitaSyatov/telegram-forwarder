Родительский репозиторий для автоматизации запуска backend и sender части приложения TelegramForwarder

Приложение предназначено для "вылавливания" сообщений по определенным словам из публичных групп.
Для того чтобы получать сообщения, нужно добавить через backend (через бота) подписку на публичную группу.

Разворачиваем на хостинге:

- git clone https://github.com/lashnag/telegram-forwarder.git
- cd telegram-forwarder
- git submodule update --init --recursive
- добавляем свой файл .env с настройками окружения
- устанавливаем python
- cd SenderApi
- pip install -r requirements.txt
- cd app
- python save_session.py
- Вводим Api Id, Api Hash, телефон и код подтверждения
- В корневой папке запускаем docker-compose up


Статья про хостинг для тг ботов:
https://www.google.com/amp/s/habr.com/ru/amp/publications/733010/