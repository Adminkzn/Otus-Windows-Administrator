## Домашнее задание №6
#### IIS сервер

Цель:
Обслуживать веб сервер от Microsoft;

#### Установите службу IIS

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/1.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/2.jpg?raw=true)

#### Откройте порты 80 и 443 в брандмауэре для входящего трафика.

Выполним 2 команды в PowerShell:
New-NetFirewallRule -DisplayName HTTP80 -Protocol TCP -LocalPort 80 -Action Allow
New-NetFirewallRule -DisplayName HTTPS443 -Protocol TCP -LocalPort 443 -Action Allow

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/3.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/4.jpg?raw=true)

#### Создайте HTML-страницу с названием курса и разместите её в IIS на порту 80.

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/6.jpg?raw=true)

#### Создайте HTML-страницу с фамилией и разместите её в IIS на порту 443, Назначьте на порт 443 сертификат от центра сертификации (CA).

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/9.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab6/8.jpg?raw=true)


