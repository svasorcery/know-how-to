# Фикс приложений Adobe для разрешения 4k UltraHD на ОС Windows 7 и выше

![Image of Adobe apps and 4k](https://github.com/svasorcery/know-how-to/blob/master/images/adobe-4k.png)

### Шаг 1: Запись в реестре для запуска сторонних файлов манифеста

###### *Вариант А:*
- Нажать `Win+R`;
- Ввести: `regedit`;
- Перейти в каталог: `HKEY_LOCAL_MACHINE > SOFTWARE > Microsoft > Windows > CurrentVersion > SideBySide`;
- Нажать правой кнопкой на каталог `SideBySide`;
- Выбрать: `New > DWORD (32-bit) Value`;
- Задать имя: `PreferExternalManifest`;
- Задать значение: `1` и выбрать тип `Decimal (Десятичное)`;

###### *Вариант Б:*
- [Скачать файл](https://github.com/svasorcery/know-how-to/blob/master/files/adobe-4k-monitor-fix.reg) и запустить, согласившись на внесение изменени в реестр Windows;


### Шаг 2: Добавление файла манифеста

- [Скачать файл](https://github.com/svasorcery/know-how-to/blob/master/files/photoshop.exe.manifest) манифеста на диск;
- Открыть каталог программы от Adobe, например, Photoshop: `C:\Program Files\Adobe\Photoshop`;
- Скопировать файл в каталог программы;
- Задать имя файла следующим образом: `<имя_исполняемого_файла_программы>.exe.manifest`. В нашем примере это: `photoshop.exe.manifest`;
- Запустить программу!
