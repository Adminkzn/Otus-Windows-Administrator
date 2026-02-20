## Домашнее задание №3
##### Парольная политика и логирование

Цель:
Разграничивать парольную политику для услиление безопасности;
Производить поиск по логам информации по изменению пароля;

------------


##### Создать парольные политики для OU employes, manager, finance на длину пароля 8, 16, 24

Создаем группу безопасности для каждого OU и добавляем туда пользователей соответсвующего OU

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab3/4.jpg?raw=true)

Создаем пораметры паролей для каждой группы

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab3/5.jpg?raw=true)

Аналогично для каждой группы 

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab3/6.jpg?raw=true)

------------


##### Вывести парольную политику для пользователя в ou manager с помощью Powershell

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab3/7.jpg?raw=true)

------------

##### Настроить гпо по логированию


------------

##### создать gpo с рандомным именем, включить сбросить пароль пользователю в OU employes, даллее найти лог по изменению в оснастке mmc и вывести результат по id лога в powershell

