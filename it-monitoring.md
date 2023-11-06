# Домашнее задание к занятию "`Обзор систем ИТ-мониторинга`" - `Свирин Марк`

---
 
### Задание 1

Создайте виртуальную машину в Yandex Compute Cloud и с помощью Yandex Monitoring создайте дашборд, на котором будет видно загрузку процессора.

#### Процесс выполнения
1. В окне браузера откройте облачную платформу Yandex Cloud
2. Перейдите в раздел "Все сервисы" > "Инфраструктура и сеть" > "Compute Cloud"
3. Нажмите на синюю кнопку "Создать ВМ" в правом верхнем углу окна браузера
4. Задайте имя виртуальной машины. Используйте английские буквы и цифры.
5. Выберите операционную систему Debian 11
6. Установите объём HDD равный 3ГБ
7. Выберите платформу Intel Ice Lake
8. Установите количество vCPU равное 2
9. Установите гарантированную долю vCPU равную 20%
10. Задайте количество RAM равное 1ГБ
11. Поставьте галочку "Прерываемая"
12. В разделе "Доступ" выберите сервисный аккаунт с ролью monitoring.editor. Если такого аккаунта нету, нажмите на кнопку "Создать новый". Задайте имя аккаунта английскими буквами, напротив надписи "Роли в каталоге" нажмите на знак "плюс". Прокручивая колесо мыши на себя, найдите роль monitoring.editor и нажмите на неё левой кнопкой мыши. Теперь вы сможете найти только что созданную роль в выпадающем списке аккаунтов.
13. Задайте логин учётной записи вашей виртуальной машины
14. Вставьте публичный SHH-ключ в поле SSH-ключ. Если этого ключа у вас нету, создайте его с помощью утилиты PuTTYgen
15. Поставьте галочку "Установить" в пункте "Агент сбора метрик"
16. Нажмите на синюю кнопку "Создать ВМ"
17. Перейдите в раздел "Все сервисы" > "Инфраструктура и сеть" > "Monitoring"
18. Нажмите на кнопку "Создать дашборд", расположенную в разделе "Возможности сервиса" > "Дашборды"
19. В открывшемся окне в разделе "Добавить виджет" нажмите на "График"
20. Пред вам предстанет конструктор запросов, выберите "Запрос А"
21. В параметре service конструктора запросов выберите Compute Cloud
22. В появившемся параметре name конструктора запросов выберите cpu_utilization
23. Поправьте диапазон времени отрисовки графика нажав на кнопку "Сейчас" в верху экрана, левее кнопок 3m, 1h, 1d, 1w, "Отменить".
24. Нажмите на кнопку "Сохранить" в правом верхнем углу экрана
25. Задайте имя дашборда, если появится окно ввода имени дашборда
26. Сделайте скриншот

![image](https://github.com/svmarkst/netology-hw/assets/110044256/78bdc0e1-7cd2-42f1-88f1-39b9b1ccd91d)



#### Требования к результату
* прикрепите в файл README.md скриншот вашего дашборда в Yandex Monitoring с мониторингом загрузки процессора виртуальной машины   

---

---

### Задание 2 со звёздочкой*
*Это дополнительное задание. Его можно не выполнять. Это не повлияет на зачёт. Вы можете его выполнить, если хотите глубже разобраться в материале.*

С помощью Yandex Monitoring сделайте 2 алерта на загрузку процессора: WARN и ALARM. Создайте уведомление по e-mail.
![image](https://github.com/svmarkst/netology-hw/assets/110044256/e3e7522e-ac67-40d7-81ce-c2054b3006fa)
![image](https://github.com/svmarkst/netology-hw/assets/110044256/1580bfa9-e4f3-46c3-a699-e8c69b4094e2)

![image](https://github.com/svmarkst/netology-hw/assets/110044256/feec0def-f97e-4269-9375-a71c61dd79d3)

Вроде как всё настроено корректно, но, к сожалению, получить алерт так и не удалось, хотя систему нагрузил под завязку. Не знаю, почему.
А ещё часто алерты и каналы удалялись самопроизвольно и приходилось всё создавать заново.


#### Требования к результату
* прикрепите в файл README.md скриншот уведомления в Yandex Monitoring 