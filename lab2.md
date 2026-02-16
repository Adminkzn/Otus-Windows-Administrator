## Домашнее задание №2
#### Групповые политики

Цель:
Настравиать и котролировать инфраструкту с помощью GPO;
Решать рутинные задачи с помощью Powershell;

------------

#####  создайте в оснастке ad ou employes, manager, finance по одному пользователю

![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/1.jpg?raw=true)

##### создать GPO на каждый OU указанный выше который будет создать txt файл на рабочем столе employes.manager,finance соотвествено имени OU=файл

Создаем и расшариваем папку, создаем в ней текстовый файл 
![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/4.jpg?raw=true)

Создаем политики в OU
![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/2.jpg?raw=true)

Настройка политик
![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/3.jpg?raw=true)

##### вывести результат gpo в cmd под любым пользователем
команда gpresult /r
![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/5.jpg?raw=true)

##### вывести информацию по любому пользователю через powershell
![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/6.jpg?raw=true)

##### заблокировать всех пользоватей в ou finance с помощью powershell
команда Get-ADUser -SearchBase "OU=Finance,DC=domain,DC=local" -Filter * | Disable-ADAccount
![](https://github.com/Adminkzn/Otus-Windows-Administrator/blob/main/img/lab2/8.jpg?raw=true)

