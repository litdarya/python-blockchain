# python-blockchain
Simple blockchain implementation for fun and a network course

# Документация

## block.py
block.py -- нода сети.

Флаги:

-s -- сервер для регистрации нод

-m -- указывает, явлется ли нода мастер-нодой (нужно для тестирования и показа, нода, которая первая стала мастером, получает 100 монет)


Если приватный и публичный ключи есть в папке с block.py, то используются они, иначе создаются новые.


/balance - баланс ноды


/whoami - публичный ключ ноды


/chain - цепочка ноды в данный момент

## server.py
Сервер, который регистрирует ноды. Получить список всех нод с их публичными ключами можно с помощью /getall.
Также серверу присылают логи, необходимые для сбора информации. Они записываются в папку tmp_logs.

## miner.py
Запуская скрипт, участник сети становится майнером.

Флаги:

 -a -- адрес ноды
 
 
 -i -- (необязательный) сколько секунд ждать между майнингом (по умолчанию, 5)
 
 ## sender.py
 Отправка транзакции.
 
 
 -p -- порт ноды, которая отправляет
 
 
 -r -- публичный ключ получателя
 
 
 -a -- сумма
 
 
 
 (при запуске на контейнере нужно использовать source ~/project/venv/bin/activate)
