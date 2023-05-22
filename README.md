# Zabbix 9-02

Задание 1
Установите Zabbix Server с веб-интерфейсом.

Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. Установите PostgreSQL. Для установки достаточна та версия что есть в системном репозитороии Debian 11
3. Пользуясь конфигуратором комманд с официального сайта, составьте набор команд для установки последней версии Zabbix с поддержкой PostgreSQL и Apache
4. Выполните все необходимые команды для установки Zabbix Server и Zabbix Web Server

Требования к результатам:
1. Прикрепите в файл README.md скриншот авторизации в админке
2. Приложите в файл README.md текст использованных команд в GitHub


![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/bcf7d00c-a0a3-4c00-89a7-a65ff9600fbc)








Задание 2
Установите Zabbix Agent на два хоста.

Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. Установите Zabbix Agent на 2 виртмашины, одной из них может быть ваш Zabbix Server
3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов
4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera
Проверьте что в разделе Latest Data начали появляться данные с добавленных агентов
Требования к результаты
1. Приложите в файл README.md скриншот раздела Configuration > Hosts, где видно, что агенты подключены к серверу
2. Приложите в файл README.md скриншот лога zabbix agent, где видно, что он работает с сервером
3. Приложите в файл README.md скриншот раздела Monitoring > Latest data для обоих хостов, где видны поступающие от агентов данные.
4. Приложите в файл README.md текст использованных команд в GitHub.

1. Установил zabbix-agent на 3 машины.

![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/18eaab67-5a5b-49ca-b2d4-b9f1197264e0)

2. Логи.
vm1
![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/4d6c8033-b7f3-4484-8c52-17e1b76344e8)

vm2
![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/1055c93c-8497-4e77-8efd-3791ba9049dd)

debian4
![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/95b5df17-d519-45b8-9937-69f922aea997)

3. Monitoring > Latest data

![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/b64a2dc3-9bfd-4f79-b3a3-874077edef61)



