# Лабораторная работа №1

## Задание 1 
Создайте файл с названием “my_first_script.sh”.
Внесите в него следующий текст:
#! /bin/bash
echo “Hello, world!”

## Решение:  
<a href="https://imgbb.com/"><img src="https://i.ibb.co/4PNvpX3/2022-09-06-09-23-38.png" alt="2022-09-06-09-23-38" border="0"></a>
## ВывоK&
<a href="https://ibb.co/hmhZnjW"><img src="https://i.ibb.co/bKq2yZB/2022-09-06-09-25-14.png" alt="2022-09-06-09-25-14" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'></a><br />



## Задание 2 
Напишите скрипт на bash, который принимает на вход два аргумента
и выводит на экран строку следующего вида:


Arguments are: $1=первый_аргумент $2=второй_аргумент

Например, если ваш скрипт называется ./script.sh, то при запуске его
./script.sh one two на экране должно появиться:

Arguments are: $1=one $2=two

а при запуске ./script.sh three four будет:

Arguments are: $1=three $2=four
## Решение: 
<a href="https://imgbb.com/"><img src="https://i.ibb.co/3sndGPT/2022-09-06-09-29-18.png" alt="2022-09-06-09-29-18" border="0"></a>
## Вывод:
<a href="https://imgbb.com/"><img src="https://i.ibb.co/k63HQ1m/2022-09-06-09-28-42.png" alt="2022-09-06-09-28-42" border="0"></a>


## Задание 3 
Напишите скрипт на bash, который ожидает ввода с клавиатуры один
аргумент (целое число от 0 до бесконечности), который будет
обозначать число студентов в аудитории. В зависимости от значения
числа нужно вывести разные сообщения.


## Решение:
<a href="https://ibb.co/cNqzQD3"><img src="https://i.ibb.co/sF7LqyR/2022-09-06-09-32-47.png" alt="2022-09-06-09-32-47" border="0"></a>
## Вывод: 
<a href="https://imgbb.com/"><img src="https://i.ibb.co/j6ZZ6bD/2022-09-06-09-33-21.png" alt="2022-09-06-09-33-21" border="0"></a>



## Задание 4 
Напишите скрипт на bash, который будет определять в какую возрастную группу
попадают пользователи. При запуске скрипт должен вывести сообщение "enter
your name:" и ждать от пользователя ввода имени (используйте read, чтобы
прочитать его). Когда имя введено, то скрипт должен написать "enter your age:"
и ждать ввода возраста (опять нужен read). Когда возраст введен, скрипт пишет
на экран "<Имя>, your group is <группа>", где <группа> определяется на основе
возраста по следующим правилам:

• младше либо равно 16: "child",

• от 17 до 25 (включительно): "youth",

• старше 25: "adult".

После этого скрипт опять выводит сообщение "enter your name:" и всё
начинается по новой. Если в какой-то момент работы скрипта будет введено
пустое имя или возраст 0, то скрипт должен написать на экран "bye" и
закончить свою работу.
## Решение: 
<a href="https://imgbb.com/"><img src="https://i.ibb.co/GWswZLv/2022-09-06-09-35-19.png" alt="2022-09-06-09-35-19" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'></a><br />
## Вывоl^
<a href="https://ibb.co/d2HY6W6"><img src="https://i.ibb.co/T8N3RvR/2022-09-06-09-37-54.png" alt="2022-09-06-09-37-54" border="0"></a>



## Задание 5 
Напишите скрипт на bash, который будет искать наибольший общий делитель
(НОД, greatest common divisor, GCD) двух чисел.
После ввода чисел скрипт считает их НОД и выводит на экран
сообщение "GCD is <посчитанное значение>", например, для чисел 15 и 25
это будет "GCD is 5". После этого скрипт опять входит в режим ожидания двух
натуральных чисел. Если в какой-то момент работы пользователь ввел вместо
этого пустую строку, то нужно написать на экран "bye" и закончить свою
работу.

Вычисление НОД несложно реализовать с помощью алгоритма Евклида. Вам
нужно написать функцию gcd, которая принимает на вход два аргумента
(назовем их M и N). Если аргументы равны, то мы нашли НОД -- он
равен M (или N), нужно выводить соответствующее сообщение на экран (см.
выше). Иначе нужно сравнить аргументы между собой. Если M больше N, то
запускаем ту же функцию gcd, но в качестве первого аргумента передаем (M-
N), а в качестве второго N. Если же наоборот, M меньше N, то запускаем
функцию gcd с первым аргументом M, а вторым (N-M).
