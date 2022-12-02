# Лабораторная работа №5 - ML-агент в экономической системе
Отчет по лабораторной работе #5 выполнил(а):
- Кошелева Татьяна Алексеевна
- НМТ-213929

Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)


## Цель работы
Интеграция экономической системы в проект Unity и обучение ML-агента.

## Задание 1
### Измените параметры файла yaml-агента и определите какие параметры и как влияют на обучение модели.
Ход работы:
- Открываем проект в Unity и переподключаем ML Agents и ML Agents Extensions через Package Manager. Активируем виртуальное пространство с помощью Anaconda Prompt и запускаем обучение ML-агента.

![1](https://user-images.githubusercontent.com/114426437/205327605-07277134-96d0-4772-a3dc-56f16f3b9c5d.png)

![2](https://user-images.githubusercontent.com/114426437/205327863-8370631e-5e29-4e23-9abe-79fed840329e.png)

![3](https://user-images.githubusercontent.com/114426437/205327958-5d1d190a-13e9-42f6-9731-39d07b5443b9.png)

![4](https://user-images.githubusercontent.com/114426437/205328103-f345bba7-a274-41af-8596-2bcc3f6564e1.png)


- После обучения ML-агента устанавливаем виртуальную среду TensorFlow и открываем TensorBoard с графиками результатов обучения.

График до изменений:

![5](https://user-images.githubusercontent.com/114426437/205332459-bf06dc20-3abf-48f5-814d-b6b9246670c2.png)

Изменили параметр `num_layers` с 2 до 4:

![6](https://user-images.githubusercontent.com/114426437/205334329-4f3fb8d5-c310-4652-b9e7-a0ad772ccfdb.png)

Уменьшили параметр `lambd` с 0,99 до 0,85:

![9](https://user-images.githubusercontent.com/114426437/205342325-83792c54-97be-4cdf-8daf-1203fad9b72f.png)

Увеличили `epsilon` с 0,2 до 0,5:

![8](https://user-images.githubusercontent.com/114426437/205340383-984ed04e-0634-4c49-8701-2959e0d896cb.png)

Изменили `batch_size` с 10 до 20:

![7](https://user-images.githubusercontent.com/114426437/205335396-bccbfffa-9efe-48a8-878b-1fb3d20167e0.png)

При изменении `lambd` значение `entropy` радикально понижалось на графике. Также, при изменении остальных значений, график `entropy` растет значительно быстрее, чем при оригинальных значениях. Самым удачным можно назвать изменение `batch_size`, т.к все графики растут больше, чем при других изменениях и даже больше, чем при значениях до изменений.


## Выводы

В данной лабораторной работе мы научились интегрировать экономическую систему в Unity и обучать ML-агента с ней работать.

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
