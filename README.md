# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #4 выполнил(а):
- Чигирев Алексей Андреевич		
- НМТ210509
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | # | 20 |
| Задание 3 | # | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
познакомиться с программными средствами для создания системы машинного обучения и ее интеграции в Unity.

## Задание 1
### В проекте Unity реализовать перцептрон, который умеет производить вычисления: OR,AND,NAND,XOR
- Создаём пустой проект, добавляем Game Object и подключаем к нему заранее скачанный Perceptron
- ![image](https://user-images.githubusercontent.com/114508818/205078294-f9ad7e8e-d141-4f99-8e2f-dc45910e5d7e.png)
- Заполняем таблицу логических операций 
 # Проверка корректности работы операции OR:
- Заполнил таблицу для операции OR, и после запуска увидел, что программа выдала ноль ошибок, а значит обучилась, после четырёх эпох обучений
![image](https://user-images.githubusercontent.com/114508818/205081945-5b9bcb6f-eee8-470d-bd6a-195176483d65.png)
 # Проверка корректности работы операции AND:
 - После запуска с пятью эпохами обучения Total Error равняется трём, а значит программа не обучилась
  ![image](https://user-images.githubusercontent.com/114508818/205089164-09d4b470-ab7e-4c67-861c-9a39f9bbae42.png)
  - Повторим ту же процедуру с шестью эпохами обучения:
 ![image](https://user-images.githubusercontent.com/114508818/205088469-95bdb8af-4231-4ac8-987b-66b74e4688bf.png)
 - После запуска увидел, что программа выдала ноль ошибок, а значит обучилась, после шести эпох обучений
 # Проверка корректности работы операции NAND:
 - С пятью эпохами обучения Total Error не равняется нулю 
 - ![image](https://user-images.githubusercontent.com/114508818/205094356-865e768e-a79b-48d6-a63a-e181b6692cf9.png)
 - ![image](https://user-images.githubusercontent.com/114508818/205094038-f468d868-627f-4b4d-a2e8-67e427eeab54.png)
 - Для операции NAND хватило 6 эпох обучений, количество ошибок равняется нулю
 - ![image](https://user-images.githubusercontent.com/114508818/205094617-b0c84f00-4890-49b7-bb6b-75feb80c770e.png)
 - ![image](https://user-images.githubusercontent.com/114508818/205094670-1bede26d-e35b-47c4-b6f0-075ea2f0619a.png) 


 # Проверка корректности работы операции XOR: 
- Проверяем с 1 эпохой
- ![image](https://user-images.githubusercontent.com/114508818/205095688-fbff9f7c-eeae-4015-9a8f-e3104f7d19c1.png)
- 2 эпохи
- ![image](https://user-images.githubusercontent.com/114508818/205095862-bdad6d24-d949-4872-acb9-43e38492d3c3.png)
- 4 эпохи
- ![image](https://user-images.githubusercontent.com/114508818/205096147-abc73c96-ba94-4489-ac61-11d21735d138.png)
- 6 эпох
- ![image](https://user-images.githubusercontent.com/114508818/205096492-a8891af7-f339-4eac-8faf-084000d71ada.png)
- Каждый раз количество ошибок не равно нулю, по той причине, что Перцептон не может обучиться нелинейной операции, из-за того, что XOR не является линейной функцией.
## Выводы

 Я познакомился с принципами действия Перцептона и его возможностями в логических операциях

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
