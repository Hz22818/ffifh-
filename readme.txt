Привет! Для начала, чтобы установить Python, читай мануал - t.me/prince_python/22

После установки Python, тебе нужно установить модули - 

pip install peewee==3.16.3
pip install pysocks==1.7.1
pip install telethon==1.23.0
pip install aiogram==2.16.0
pip install opentele==1.15.1
pip install phonenumbers==8.13.18
pip install aiosqlite==0.19.0

Просто вводи эти команды в консоль, и твой скрипт 100% заработает, если не заработает, пиши - t.me/contact_prince_bot

КАК НАСТРОИТЬ КОНФИГ

Конфиг, по идее, настраивается за 5 минут, но, 
если вы впервые видете Python и подобные скрипты, то это займет чуть больше времени;)

Начнем! Сначала нам нужно перейти на my.telegram.org/auth и авторизировать свой аккаунт,
после чего создать приложение, чтобы получить API. Полно гайдов в интернете на эту тему, 
3 минуты времени почитать

После создания приложения вставляем api_id и api_hash в конфиг бота. (api_id пишем без ковычек, api_hash - с ковычками)

Теперь, нам нужно создать самого бота, на который мы будем лить траффик.
Заходим в @bot_father и пишем команду /newbot, после чего следуем его инструкциям и в конце получаем
сообщение с токеном нашего бота. Он выглядит примерно так - "68293737666:AAFuGHYwTXPD6M9-TslKjddLuG_nKtD51Jw"

Теперь, когда мы вставили токен бота в конфиг, нам нужно получить свой телеграм-айди, 
чтобы подключить админку. Пишем боту - @FIND_MY_ID_BOT и получаем свой айди, 
пишем в конфиг нам админ айди (без ковычек) и переходим к следующему пункту

logs, это айди чата, в который нам будут приходить все сессии. Добавляем @FIND_MY_ID_BOT в любой чат и пишем команду /id@FIND_MY_ID_BOT,
после чего бот отправит сообщение с ID чата. Записываем его в конфиг в строчку logs с минусом и без ковычек, 
должно быть примерно так: logs = -1001920261773
Если не вставить это, то бот просто не будет уведомлять вас о новых мамонтах.

Теперь к функциям фишинга.

botdelete - это удаление переписки с ботом после авторизации в аккаунт мамонта
twofa_set - функция, которая ставит 2FA аутентификацию на аккаунт мамонта, если False, то работать не будет. 
Чтобы работало, надо изменить на True (также и со всеми остальными функциями)

twofa_current - функция, которая изменяет 2FA, если он уже стоит.
twopass_set - это будущий пароль, который будет ставиться на аккаунт мамонта, если twofa_set и twofa_current включены (= True)
hint_set - это подсказка от 2FA, не очень полезная функция, но чтобы поиздеваться над мамонтом пойдет)

chango - подписка на чат\канал после авторизации в сессию, 
ниже (в userchannel) напишите имя чата или канала, на который нужно автоматически подписаться после авторизации

proxyuse - Использование прокси, те, кто понимают о чем я говорю, поймут как это использовать.

spams - Спам после авторизации (как всегда, если = False, то выключено, чтобы включить ставим = True)
SPAM_MSG - Сообщение, которое будет рассылаться

device_model - после этого идет ювелирная работа, которая может привести к плохим последствиям, если настроить ее неправильно,
Поэтому, советую не трогать, я настроил вроде хорошо.

Про функционал админки:
существуют две основные команды, это /stat (бот пишет, сколько пользователей в боте) 
и команда /spam (она используется для рассылки, спама или рекламы)
Также админу приходят уведомления о новых пользователях 
(настроено так, что присылается только тогда, когда пользователь захотел воспользоваться наживкой и перешел к стадии фишинга)
и о мамонтах, которые поделились номером телефона с ботом, но пока еще не замамонтились.

На этом настройка конфига закончена, чтобы запустить скрипт пишем в консоль Python gpt.py и пишем /start боту.

Чтобы настроить саппорт-бота, нам нужно заменить bot_token на токен нашего бота (нового, специально для тех поддержки) и админ айди, я уже рассказывал как это сделать.
Если вы хотите настроить свои категории, то просто перепишите их в category, но их обязательно должно быть 4!

Больше подобных скриптов - t.me/prince_python









