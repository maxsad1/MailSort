<h1 align="center">
  <span style="color: #3498db;">✉️</span> <span style="font-weight: bold; color: #2c3e50;">MailSort.exe:</span> <span style="color: #2ecc71;">Ваш надежный почтовый ассистент!</span>
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Version-3.2.1-blue" alt="Version 3.2.1"/>
</p>


<hr style="border: 1px solid #e74c3c;">

## <span style="color: #3498db;">📝</span> Описание

<p>
    <code>MailSort.exe</code> – это мощная утилита для автоматической сортировки писем в MS Outlook, разработанная командой <span style="font-weight: bold; color: #9b59b6;">KilocodE</span>. Она поможет вам навести порядок в вашей электронной почте, автоматизируя рутинные задачи по сортировке и архивированию.
</p>
<p>
Наша утилита не просто инструмент, это ваш личный почтовый ассистент, который работает незаметно и эффективно, освобождая ваше время для более важных дел. Мы в <span style="font-weight: bold; color: #9b59b6;">KilocodE</span> стремимся к тому, чтобы наши программы были не только функциональными, но и удобными в использовании.
</p>

## <span style="color: #2ecc71;">✨</span> Основные возможности:

-   <span style="color: #3498db;">**Автоматическая сортировка писем:**</span>
    -   Интеллектуальное перемещение новых писем из папки "Входящие" в структурированные подпапки в папке "Темы" на основе правил, определенных в конфигурационных INI-файлах.
    -   Поддержка сортировки по нескольким условиям:
        -   Отправитель
        -   Ключевые слова в тексте письма
        -   Частичное совпадение темы письма
    -   Автоматическое создание новых папок, если требуемая папка еще не существует.
    -   Ограничение длины имени создаваемой папки для лучшей организации.
-   <span style="color: #3498db;">**Интеллектуальное объединение похожих папок:**</span>
    -   Слияние папок с похожими именами в папках "Темы" и "Архив", что способствует лучшей организации вашей почты.
    -   Настраиваемый порог схожести имен папок, позволяющий точно настроить процесс объединения.
    -   Возможность исключения определенных папок из процесса объединения.
    -   Автоматическое перемещение писем из объединяемых папок в целевую.
    -   Удаление пустых исходных папок после слияния, что поддерживает порядок.
-   <span style="color: #3498db;">**Умная архивация прочитанных писем:**</span>
    -   Автоматическое перемещение папок, где все письма прочитаны, из папки "Темы" в папку "Архив".
    -   Возможность исключения определенных папок из процесса архивации.
-   <span style="color: #3498db;">**Архивация по дате:**</span>
    -   Перемещение папок из папки "Архив" в подпапки, структурированные по годам, месяцам и неделям (год/месяц/неделя), используя дату получения первого письма в папке.
    -   Если в папке нет писем, используется текущая дата, обеспечивая логическую организацию архива.
-   <span style="color: #3498db;">**Восстановление папок из архива:**</span>
    -   Автоматическое перемещение папок с непрочитанными письмами из папки "Архив" обратно в папку "Темы", гарантируя, что важные сообщения не будут забыты.
-  <span style="color: #3498db;">**Автоматическая очистка пустых папок:**</span>
    -   Удаление пустых папок (без писем и подпапок) в папках "Темы" и "Архив", что помогает поддерживать чистоту почтового ящика.
    -   Исключение определенных папок из процесса удаления, предоставляя гибкость в управлении вашими папками.
-   <span style="color: #3498db;">**Гибкая настройка через INI файлы:**</span>
    -   Вся конфигурация утилиты хранится в INI файлах, что позволяет вам легко настроить работу <code>MailSort.exe</code> под свои нужды.
-   <span style="color: #3498db;">**Подробное логирование:**</span>
    -   Ведение журнала всех действий утилиты в файле `mailsort_log.txt` с подробными записями о перемещении писем и возникших ошибках.
    -   Настройка размера лог-файла, что дает возможность контролировать объем хранимых данных.
    -   Поддержка вывода сообщений в консоль для отслеживания работы в режиме реального времени.
-   <span style="color: #3498db;">**Лицензирование:**</span>
    -  Расширенный функционал:  удаление пустых папок, архивация, объединение, восстановление папок  доступен только при наличии лицензии (key-файл).

## <span style="color: #f39c12;"> ⚙️</span> Управление из командной строки

<p><code>MailSort.exe</code> поддерживает следующие аргументы командной строки:</p>

-   <code>-inst</code>: Первый запуск. Создает INI-файлы, key-файл и BAT-файл для запуска по расписанию.
-   <code>-key</code>: Создает key-файл (пробный).
-   <code>-ini</code>: Создает INI-файлы.
-   <code>-bat</code>: Создает BAT-файл для запуска по расписанию.
-   <code>-start</code>: Добавляет задание в планировщик задач Windows для запуска каждые 30 минут.
-   <code>-stop</code>: Удаляет задание из планировщика задач Windows.
-   <code>-info</code>: Выводит справочную информацию в файл.
-   <code>-help</code>: Выводит справку по использованию.

## <span style="color: #27ae60;">🚀</span> Как начать

1.  **Скачайте** исполняемый файл `MailSort.exe`.
2.  **Первый запуск:** Запустите `MailSort.exe -inst`. Утилита создаст необходимые INI-файлы, key-файл и BAT-файл для дальнейшей работы.
3.  **Настройте INI-файлы:** Откройте `mailsort.ini` и `mailsort_rules.ini` и отредактируйте параметры под свои потребности.
4.  **Запуск вручную:** Запустите `MailSort.exe` без аргументов для однократной сортировки.
5.  **Запуск по расписанию:** Запустите `mailsort_start.bat` для автоматического запуска утилиты каждые 30 минут.
    -   Для автоматизации с помощью планировщика заданий:
        1.  Запустите `MailSort.exe -start` для добавления задания в планировщик задач.

## <span style="color: #9b59b6;">🗂️</span> Файлы конфигурации

-   `mailsort.ini`: Содержит основные настройки утилиты, включая пути к файлам, параметры сортировки и архивирования.
-   `mailsort_rules.ini`: Определяет правила сортировки писем, включая ключевые слова для поиска в темах и телах писем.
-   `mailsort_log.txt`: Лог-файл, в котором утилита записывает свои действия и возможные ошибки.
-   `readme.txt`: Содержит справочную информацию об утилите.
-  `.key`: Файл лицензии.

## <span style="color: #e67e22;">🗣️</span> Обратная связь

<p>Если у вас возникли вопросы или предложения, пожалуйста, свяжитесь с нами по адресу: <a href="mailto:KilocodE@yandex.ru">KilocodE@yandex.ru</a>.</p>

<hr style="border: 1px solid #e74c3c;">
<p align="center">
  <span style="font-weight: bold; color: #2c3e50;">Спасибо за выбор</span> <span style="color: #2ecc71;">MailSort.exe</span>!<span style="color: #3498db;"> 🎉</span>
</p>
