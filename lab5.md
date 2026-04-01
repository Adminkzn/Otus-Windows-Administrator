## Домашнее задание №5
#### RDS сервер

Цель:
Создать rds сервер, для организации удаленного доступа к рессурсам компании;

#### Установите службу терминального сервера (RDS)
Устанавливаем службу  терминалов с компанентами - узел сеансов, сервер лицензирования и шлюз на новую вертуальную машину SRV-RDS

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/1.jpg?raw=true)

#### Создайте группу безопасности и настройте правила для входа по RDP. Добавьте в эту группу пользователя из OU Manager.

Включаем группу безопасности Manager в группу безопасности Пользователи удаленого рабочего стола

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/16.jpg?raw=true)

Создаем новую вертуальную машину SRV-RDP-MANAGER и разрешаем удаленый доступ группе безопасности Manager

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/14.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/15.jpg?raw=true)

Создаем новую группу устройств в Диспечере шлюза удаленого рабочего стола и включаем в нее SRV-RDP-MANAGER

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/23.jpg?raw=true)

Создаем новую политику в Диспечере шлюза удаленого рабочего стола 

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/24.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/25.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/26.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/27.jpg?raw=true)

Создаем сертификат и устанавливаем его на PC1 

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/28.jpg?raw=true)

#### Подключитесь к серверу по RDP как пользователь из OU Manager и зафиксируйте информацию о входе в системе логов.

C компьютера PC1 подключаемся к SRV-RDP-MANAGER

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/30.jpg?raw=true)

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab5/29.jpg?raw=true)

В качестве теста разрешил удаленый доступ группе безопасности Manager на сервер SRV-RDS, подключится не удалось политики безопасности шлюза работают 
