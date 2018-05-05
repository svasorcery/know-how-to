# Установка MongoDB Server в ОС Windows

![MongoDBLogo](https://github.com/svasorcery/know-how-to/blob/master/images/mongodb-logo.png)

### Установка сервера
1. Скачать дистрибутив сервера с оф. сайта: https://www.mongodb.com/download-center ;
2. Установить в стандартную папку (`C:\Program Files\MongoDB\Server`);
3. Перенести файлы из стандартной папки в корневую: `C:\mongodb\server`;

### Конфигурация сервера
4. В папке `C:\mongodb` создать папки `data` и `log`;
5. Создать файл конфигурации `C:\mongodb\mongo.config` и добавить в него:
```xml
##store data
dbpath=C:\mongodb\data 
##Log File
logpath=C:\mongodb\log\mongo.log 
##log read and write operations
diaglog=3
```

### Автозапуск сервера
6. Запустить консоль `cmd` от имени администратора;
7. Войти в папку с сервером: `cd c:\mongodb\server\bin`;
8. Выполнить команду: `mongod.exe --config C:\mongodb\mongo.config –install`;
9. Открыть `Панель управления (Control Panel) > Администрирование (Administration) > Службы (Services)`;
10. Найти сервис `MongoDB` и нажать на кнопку `Запустить`;

### Установка клиента
11. Скачать дистрибутив клиента `Robomongo`: https://robomongo.org/download ;
12. Установить `Robomongo` и запустить;
13. Создать новое подключение к локальному серверу mongodb – `127.0.0.1:27017`; 
