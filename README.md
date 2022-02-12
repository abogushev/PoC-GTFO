# PoC-GTFO

## Описание проекта
  hello world server\
  [Git Repository](git@github.com:abogushev/PoC-GTFO.git)
___
## Установка окружения (начальная инициализация)

***vagrant окружение***
```bash
mkdir vagrant
cd vagrant
vagrant init hashicorp/bionic64
vagrant up
```

***python окружение***
```bash
vagrant ssh
sud apt-get update
sudo apt-get install python3-venv
cd /vagrant
python3 -m venv venv
source venv/bin/activate
pip install flask
git clone git@github.com:abogushev/PoC-GTFO.git
```
 ___
***Запуск***

поднять vagrant, если не запущен
```
cd vagrant
vagrant up
```
запуск сервиса
```bash
vagrant ssh
cd /vagrant
sudo python PoC-GTFO/main.py &
```