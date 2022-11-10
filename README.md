# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #3 выполнил(а):
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
### Реализовать систему машинного обучения в связке Python - Google-Sheets – Unity.
- Создаём новый 3D проект в Unity
- ![image](https://user-images.githubusercontent.com/114508818/201169182-4a2e8f07-eb86-4603-8cef-ac7e9ce485c7.png)

- Добавляем в новый проект ML Agent
- ![image](https://user-images.githubusercontent.com/114508818/201176657-6998eae1-fce4-4c1a-8d17-8fb61fb62abc.png)

- Пишем серию команд в Anaconda Prompt для создания и активации нового ML-агента и для скачивания необходимых библиотек:
o mlagents 0.28.0;
o torch 1.7.1;
- ![image](https://user-images.githubusercontent.com/114508818/201176344-7c641b17-f341-4609-801e-5613b31221b2.png)
- Создаём на сцене плоскость, куб и сферу
- ![image](https://user-images.githubusercontent.com/114508818/201177889-89b0956b-edbf-4f47-af6e-95c504719926.png)
- Создаём скрипт и пишем код, который мы получили из материалов к ЛР
- ![image](https://user-images.githubusercontent.com/114508818/201178880-102c2176-3c0d-428b-bd20-63bcbc51a737.png)
- Добавляем компоненты Decision Requester, Behavior Parameters для сферы
- ![image](https://user-images.githubusercontent.com/114508818/201179081-a073da5e-0f49-4bf6-827c-5359e34d1c09.png)
- Добавляем файл конфигурации нейронной сети
behaviors:
  RollerBall:
    trainer_type: ppo
    hyperparameters:
      batch_size: 10
      buffer_size: 100
      learning_rate: 3.0e-4
      beta: 5.0e-4
      epsilon: 0.2
      lambd: 0.99
      num_epoch: 3
      learning_rate_schedule: linear
    network_settings:
      normalize: false
      hidden_units: 128
      num_layers: 2
    reward_signals:
      extrinsic:
        gamma: 0.99
        strength: 1.0
    max_steps: 500000
    time_horizon: 64
    summary_freq: 10000
- Запускаем ML-агент, и сцену в Unity
## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

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
