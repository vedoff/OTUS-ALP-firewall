# Firewall
### Реализация кнокинг, взаимодействие с маршрутизацией.
1. Запустить nginx на centralServer.
2. Добавить inetRouter2, который виден(маршрутизируется (host-only тип сети для виртуалки)) с хоста или форвардится порт через локалхост.
3. Пробросить 80й порт на inetRouter2 8080.
4. Дефолт в инет оставить через inetRouter.
5. Реализовать проход на 80й порт без маскарадинга.
6. Реализовать knocking port.
7. centralRouter может попасть на ssh inetrRouter через knock скрипт.

### Схема стенда
![](https://github.com/vedoff/firewall/blob/main/pict/Screenshot%20from%202022-03-25%2012-39-14.png)

## Реализация
Разворачиваем стенд: \
`vagrant up`

#### 1. Запустить nginx на centralServer.
`ansible-playbook nginx-play.yml`

![](https://github.com/vedoff/firewall/blob/main/pict/Screenshot%20from%202022-03-24%2017-55-17.png)

![](https://github.com/vedoff/firewall/blob/main/pict/Screenshot%20from%202022-03-24%2017-55-52.png)

### Проброс порта сайта
#### Реализоано через provision при развертывании.
- Добавить inetRouter2, который виден(маршрутизируется (host-only тип сети для виртуалки)) с хоста или форвардится порт через локалхост.
- Дефолт в инет оставить через inetRouter.
- Пробросить 80й порт на inetRouter2 8080.
- Реализовать проход на 80й порт без маскарадинга.

![](https://github.com/vedoff/firewall/blob/main/pict/Screenshot%20from%202022-03-25%2012-59-05.png)

![]()
