# Telegram-Бот @IVRBot #
- - -
###### Telegram-клиент Кафедры Исследовательской и Проектной деятельности учащихся Лицея ВШЭ ######
###### Москва, 2018

## О боте 
Telegram-бот был создан в 2018 году в рамках проектной деятельности учащихся Лицея ВШЭ. 

Цель написания Telegram-бота - создание удобного инструмента коммуникации между администрацией Кафедры и учащимися.

Бот реализован на языке Python с помощью библиотек PyTelegramBotAPI и SQLite и использует базы данных для обработки информации о зарегестрированных пользователях.

Основной код Telegram-бота доступен в файле bot_main.py. Обширное количество комментариев дает возможность использовать код в качестве учебного для тех, кто только начинает разрабатывать Telegram-ботов.

## Шаг 1. Регистрация (или вход)
![Начало работы](Screenshots/Начало.png)

Начало работы классическое - в описании сказана пара слов о том, зачем этот бот нужен, а сам он вызывается по функции /start . 

После вызова бота ID сообщения - то есть ID пользователя - анализируется ботом. Он сравнивает ID со всеми, существующими в базе данных, и уже из этого делает вывод, нужна регистрация или нет. 

Если ID оказывается новым, то пользователь переходит к процедуре регистрации. Если ID уже есть в базе данных, то в зависимости от прошлой регистрации пользователь переходит либо в меню администратора, либо в меню ученика.


Название файла  | Содержание файла
----------------|----------------------
style.css       | Пустой файл каскадной таблицы стилей, в который производится сбока необходимых стилей
reset.css       | Reset CSS от Эрика Мейера
