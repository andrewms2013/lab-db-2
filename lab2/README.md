# Лабораторна робота No 2. Практика використання серверу Redis

## Виконавець

Мироненко Андрій Станіславович. Группа КП-71

## Завдання 

[Посилання на завдання](http://scs.kpi.ua/sites/default/files/lab2_bd2-db2019_2020.pdf)

## Структура даних
Для зберігання повідомлень використана хештаблиця, так як вона дозоволяє зберігати ключ та значення. Ключем виступає id повідомлення, значенням - ім'я користувача-відправника, користувача-отримувача, текст повідомлення.

Для зберігання користувачів використана множина (Set), так як нам не є важливий їх порядок, але є важливою швидкість доступу до них.

Для черги повідомлень використувоється List, так як нам є важливий порядок доданих записів, та час додавання та вилучення, який у випадку використання List є константним


## Приклади роботи програми

Приклад відправки повідомлення 

![1](./images/1.png)

![2](./images/2.png)

Аккаунт адміністартору

![3](./images/3.png)

Приклад спаму

![4](./images/4.png)

![5](./images/5.png)

Приклад логів, які залишає додаток

![6](./images/6.png)
