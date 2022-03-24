# Firewall
### Реализация кнокинг, взаимодействие с маршрутизацией.
1. Реализовать knocking port.
2. centralRouter может попасть на ssh inetrRouter через knock скрипт.
3. Добавить inetRouter2, который виден(маршрутизируется (host-only тип сети для виртуалки)) с хоста или форвардится порт через локалхост.
4. Запустить nginx на centralServer.
5. Пробросить 80й порт на inetRouter2 8080.
6. Дефолт в инет оставить через inetRouter.
7. Реализовать проход на 80й порт без маскарадинга.

## Реализация
Разворачиваем стенд: \
`vagrant up`

