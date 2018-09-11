# Установка RabbitMQ Server в ОС Windows

![RabbitMQLogo](https://github.com/svasorcery/know-how-to/blob/master/images/rabbitmq-logo.png)

### Установка сервера
1. Скачать дистрибутив Erlang: http://www.erlang.org/downloads ;
2. Установить под административной учетной записью;
3. Скачать дистрибутив RabbitMQ Server: http://www.rabbitmq.com/download.html ;
4. Установить стандартно;

### Конфигурация сервера
5. Настройки по-умолчанию хранятся в каталоге: `%APPDATA%/RabbitMQ`;
6. Документация по конфигурации сервера: http://www.rabbitmq.com/configure.html ;
7. Командная строка: http://www.rabbitmq.com/cli.html ;

### Автозапуск сервера
8. После установки сервер настроен на автозапуск и доступен по адресу: `127.0.0.1:5672`;

### Установка клиента
9. Установка библиотеки клиента зависит от платформы разработки: https://www.rabbitmq.com/getstarted.html ;
