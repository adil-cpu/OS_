# Презентация к лабораторной работе №12

----

# Тема:
## Программирование в командном процессоре ОС UNIX. Ветвления и циклы

----

## Российский Университет Дружбы Народов

### Факультет Физико-Математических и Естественных Наук

*Дисциплина: Операционные системы*

Студент: Мухамедияр Адиль

Группа: НКНбд-01-20

Москва, 2021г.

----

### Цель работы

Изучить основы программирования в оболочке ОС UNIX. Научится писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

----

### Введение

Операции с блоками кода — ключ к структурированным и упорядоченным сценариям оболочки. Циклы и ветвления являются теми инструментальными средствами, которые предоставляют возможность достигнуть этой цели.

##### Циклы
Цикл это блок команд, который повторяется (итерируется) до тех пор, пока не будет выполнено условие выхода из цикла .

----

### Ход работы:

1. Для начало я скопировал любой текст из интернета.

![1_1.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/1_1.PNG?raw=true)

* Используя команды getopts grep, написал командный файл.

![1_2_1.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/1_2_1.PNG?raw=true)


* Данный командный файл анализирует командную строку с ключами:
 -iinputfile — прочитать данные из указанного файла;
 -ooutputfile — вывести данные в указанный файл;
 -pшаблон — указать шаблон для поиска;
 -C — различать большие и малые буквы;
 -n — выдавать номера строк.

![1_2_2.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/1_2_2.PNG?raw=true)

* После я написал слово, которую программа ищет в моем тексте, используя ключ -p.

![1_3.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/1_3.PNG?raw=true)

2. Написал на языке Си программу, которая вводит число и определяет, является ли оно больше нуля, меньше нуля или равно нулю. Затем программа завершается с помощью функции exit(n), передавая информацию о коде завершения в оболочку.

![2_1.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/2_1.PNG?raw=true)

* Командный файл вызывает эту программу и, проанализировав с помощью команды $?, выдает сообщение о том, какое число было введено.

![2_2.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/2_2.PNG?raw=true)

* Проверил свой код.

![2_3.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/2_3.PNG?raw=true)

3. Написал командный файл, создающий указанное число файлов, пронумерованных последовательно от 1 до N (например 1.tmp, 2.tmp, 3.tmp, 4.tmp и т.д.).

![3_1.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/3_1.PNG?raw=true)

* Число файлов, которые необходимо создать, передаётся в аргументы командной строки.

![3_2.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/3_2.PNG?raw=true)

* Этот же командный файл удаляет все созданные им файлы (если они существуют).


![3_3.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/3_3.PNG?raw=true)

4. Написал командный файл, который с помощью команды *tar* запаковывает в архив все файлы в указанной директории. 

![4_1.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/4_1.PNG?raw=true)

* Модифицировал его так, чтобы запаковывались только те файлы, которые были изменены менее недели тому назад (использовал команду find).

![4_2.png](https://github.com/adil-cpu/OS_/blob/main/lab12/img/4_2.PNG?raw=true)

----

### Вывод

Изучил основы программирования в оболочке ОС UNIX, научился писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

----

### Библиография

[Домашний склерозник](https://www.skleroznik.in.ua/2013/07/31/cikly-i-vetvleniya/)

----