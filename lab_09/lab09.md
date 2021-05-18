# Отчет по лабораторной работе №9

----

# Тема:
## Текстовой редактор vi

----

## Российский Университет Дружбы Народов

### Факультет Физико-Математических и Естественных Наук

*Дисциплина: Операционные системы*

Студент: Мухамедияр Адиль

Группа: НКНбд-01-20

Москва, 2021г.

----

### Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

----

### Введение

В большинстве дистрибутивов Linux в качестве текстового редактора по умолчанию устанавливается интерактивный экранный редактор vi (Visual display editor).
Редактор vi имеет три режима работы:
* командный режим — предназначен для ввода команд редактирования и навигации по редактируемому файлу;
* режим вставки — предназначен для ввода содержания редактируемого файла;
* режим последней (или командной) строки — используется для записи изменений в файл и выхода из редактора.
Для вызова редактора vi необходимо указать команду vi и имя редактируемого файла:
vi <имя_файла>
При этом в случае отсутствия файла с указанным именем будет создан такой файл.
Переход в командный режим осуществляется нажатием клавиши Esc . Для выхода из редактора vi необходимо перейти в режим последней строки: находясь в командном режиме, нажать Shift-; (по сути символ : — двоеточие), затем:
* набрать символы wq, если перед выходом из редактора требуется записать изме-
нения в файл;
* набрать символ q (или q!), если требуется выйти из редактора без сохранения.

----

### Последовательность выполнения работы
1. Ознакомиться с теоретическим материалом.
2. Ознакомиться с редактором vi.
3. Выполнить упражнения, используя команды vi.

----

### Ход работы:

#### Задание 1. Создание нового файла с использованием vi.

1. Создал каталог с именем ~/work/os/lab06.
2. Перешел во вновь созданный каталог.
3. Вызвал vi и создал файл hello.sh

![1_1.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_1.PNG?raw=true)

![1_2.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_2.PNG?raw=true)

4. Нажав клавишу i, ввел следующий текст:
#!/bin/bash
HELL=Hello
function hello {
LOCAL HELLO=World
echo $HELLO
}
echo $HELLO
hello

![1_3.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_3.PNG?raw=true)

5. Нажав клавишу Esc, перешел в командный режим, после завершения ввода текста.

![1_.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_..PNG?raw=true)

6. Нажал «:» для перехода в режим последней строки и внизу экрана появилось приглашение в виде двоеточия.

![1_4.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_4.PNG?raw=true)

7. Нажал w (записать) и q (выйти), а затем нажал клавишу Enter для сохранения текста и завершения работы.

![1_5.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_5.PNG?raw=true)

8. Сделал файл исполняемым. 

![1_6.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/1_6.PNG?raw=true)

#### Задание 2. Редактирование существующего файла.

1. Вызвал vi на редактирование файла.

![2_1.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_1.PNG?raw=true)

2. Установил курсор в конец слова HELL второй строки.

![2_2.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_2.PNG?raw=true)

3. Перешел в режим вставки и заменил на HELLO. Нажал Esc для возврата в командный режим.

![2_3.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_3.PNG?raw=true)

4. Установил курсор на четвертую строку и стёр слово LOCAL.

![2_4.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_4.PNG?raw=true)

5. Перешел в режим вставки и набрал следующий текст: local, нажала Esc для возврата в командный режим.

![2_5.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_5.PNG?raw=true)

6. Установил курсор на последней строке файла. Вставил после неё строку, содержащую следующий текст: echo $HELLO.

![2_6.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_6.PNG?raw=true)

7. Нажал Esc для перехода в командный режим.

8. Удалил последнюю строку.

![2_7.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_7.PNG?raw=true)

9. Ввел команду отмены изменений u для отмены последней команды.

![2_8.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_8.PNG?raw=true)

10. Ввел символ «:» для перехода в режим последней строки. Записал произведённые изменения и вышел из vi. 

![2_9.png](https://github.com/adil-cpu/OS_/blob/main/lab_09/img/2_9.PNG?raw=true)

----

### Вывод

Познакомился с операционной системой Linux, получил практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

----

### Библиография

[Работа с редактором vi](https://docs.altlinux.org/ru-RU/archive/2.3/html-single/junior/alt-docs-extras-linuxnovice/ch02s10.html)

## Ответы на контрольные вопросы:

1.Краткая характеристика режимов работы редактора vi:
* командный режим — предназначен для ввода команд редактирования и навигации по редактируемому файлу;
* режим вставки — предназначен для ввода содержания редактируемого файла;
* режим последней (или командной) строки — используется для записи изменений
в файл и выхода из редактора.
2. Выйти из редактора, не сохраняя произведённые изменения, можно используя клавиши «:q!» в командном режиме.
3. Краткую характеристика команд позиционирования:
* 0 (ноль) — переход в начало строки;
* $ — переход в конец строки;
* G — переход в конец файла;
* n G — переход на строку с номером n.
4. Для редактора vi словом является: пробел; буквы, находящиеся между двумя пробелами.
5. Из любого места редактируемого файла перейти в конец файла можно с помощью клавишы G и курсора вниз, а в начало – курсор вверх.
6. Краткая характеристика основных групп команд редактирования:
Вставка текста
* а — вставить текст после курсора;
* А — вставить текст в конец строки;
* i — вставить текст перед курсором;
* n i — вставить текст n раз;
* I — вставить текст в начало строки.
Вставка строки
* о — вставить строку под курсором;
* О — вставить строку над курсором.  Удаление текста
* x — удалить один символ в буфер;
* d w — удалить одно слово в буфер;
* d $ — удалить в буфер текст от курсора до конца строки;
* d 0 — удалить в буфер текст от начала строки до позиции курсора;
* d d — удалить в буфер одну строку;
* n d d — удалить в буфер n строк.  Отмена и повтор произведённых изменений
* u — отменить последнее изменение;
* . — повторить последнее изменение.
Копирование текста в буфер
* Y — скопировать строку в буфер;
* n Y — скопировать n строк в буфер;
* y w — скопировать слово в буфер.
Вставка текста из буфера
* p — вставить текст из буфера после курсора;
* P — вставить текст из буфера перед курсором.  Замена текста
* c w — заменить слово;
* n c w — заменить n слов;
* c $ — заменить текст от курсора до конца строки;
* r — заменить слово;
* R — заменить текст.
Поиск текста
* / текст — произвести поиск вперёд по тексту указанной строки символов текст;
* ? текст — произвести поиск назад по тексту указанной строки символов текст. 7. Чтобы заполнить строку символами $ можно использовать клавиши ni(вставить текст n раз).
8. Отменить некорректное действие, связанное с процессом редактирования, можно с помощью клавиши «.».
9. Характеристика основных групп команд режима последней строки:
Копирование и перемещение текста
* : n,m d — удалить строки с n по m;
* : i,j m k — переместить строки с i по j, начиная со строки k;
* : i,j t k — копировать строки с i по j в строку k;
* : i,j w имя-файла — записать строки с i по j в файл с именем имя-файла.
Запись в файл и выход из редактора
* : w — записать изменённый текст в файл, не выходя из vi;
* : w имя-файла — записать изменённый текст в новый файл с именем имяфайла;
* : w ! имя-файла — записать изменённый текст в файл с именем имяфайла;
* : w q — записать изменения в файл и выйти из vi;
* : q — выйти из редактора vi;
* : q ! — выйти из редактора без записи;
* : e ! — вернуться в командный режим, отменив все изменения, произведённые со времени последней записи.
10. Определить, не перемещая курсора, позицию, в которой заканчивается строка, можно используя клавишу $ (переход в конец строки).
11. Опции редактора vi позволяют настроить рабочую среду. Для задания опций
используется команда set (в режиме последней строки):
* : set all — вывести полный список опций;
* : set nu — вывести номера строк;
* : set list — вывести невидимые символы;
* : set ic — не учитывать при поиске, является ли символ прописным или
строчным.
Если вы хотите отказаться от использования опции, то в команде set перед именем опции надо поставить no.
12. Определить режим работы редактора vi можно по последней командной строке.
13. Взаимосвязь режимов работы редактора vi:
«Командный режим»     -     «Режим вставки»
                          \                             /
                 «Режим командной строки»