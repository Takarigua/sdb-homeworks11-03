# Домашнее задание к занятию "`ELK`" - `Марченко Вячеслав Игоревич`

---

### Задание 1

Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный.

Приведите скриншот команды 'curl -X GET 'localhost:9200/_cluster/health?pretty', сделанной на сервере с установленным Elasticsearch. Где будет виден нестандартный cluster_name.

### Ответ

1. ![clustername](https://github.com/Takarigua/sdb-homeworks11-03/blob/c7f799b8861f3d6a729f601bf59cab4b548677cd/img/cluster%20name.png)


---

### Задание 2

Установите и запустите Kibana.

Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty.

### Ответ

1. ![kibana](https://github.com/Takarigua/sdb-homeworks11-03/blob/ae06d8097d71062d9b1c74783d8a7fb52a4e0282/img/kibana.png)

---

### Задание 3

Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx.

### Ответ

1. ![logstash](https://github.com/Takarigua/sdb-homeworks11-03/blob/64ffebd9471ae04570f51628fefb2f315f917da8/img/logstash.png)
2. `Заполните здесь этапы выполнения, если требуется ....`
3. `Заполните здесь этапы выполнения, если требуется ....`
4. `Заполните здесь этапы выполнения, если требуется ....`
5. `Заполните здесь этапы выполнения, если требуется ....`
6. 

---

### Задание 4

Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx, которые были отправлены через Filebeat.

### Ответ

---

1. `Заполните здесь этапы выполнения, если требуется ....`


