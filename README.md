# Использование

Запустить playbook командой:
ansible-playbook -i inventory wordpress.yml

Будет создано две базы данных: мастер и реплика.

После успешной установки WordPress будет доступен по умолчанию по адресу:
http://192.168.0.111

Для установки на свой сервер необходимо указать в inventory адрес своего VPS и доступы. 
Перед установкой убедиться, что есть доступ к серверу по SSH.

## Структура проекта

- `inventory` - файл с определением хостов
- `wordpress.yml` - playbook
- `docker-compose.yml` - конфигурация Docker-контейнеров


