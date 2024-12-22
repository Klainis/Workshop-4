# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #4 выполнил(а):
- Усольцев Матвей Александрович
- РИ-230950
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * |  |
| Задание 2 | * |  |
| Задание 3 | # |  |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

Структура отчета

- Данные о работе: "ПЕРЦЕПТРОН", Усольцев Матвей Алексндрович, АТ-04, выполненные задания.
- Цель работы.
- Задание 1.
- Задание 2.
- Задание 3.
- Выводы.

## Цель работы
Познакомиться с перцептроном и реализовать его в проекте Unity.

## Задание 1
### Реализовать перцептрон в проекте Unity, умеющий производить логические вычисления:
- OR | дать комментарии о корректности работы
- AND | дать комментарии о корректности работы
- NAND | дать комментарии о корректности работы
- XOR | дать комментарии о корректности работы

Ход работы:
- Создал новый 2D проект на Unity
- Создал пустой объект Empty Game Object с именем `Perceptron`
- Подключил `Perceptron.cs` к пустому объекту

  ### OR
  - Настроил `TrainingSet` на обучение вычисления логического `ИЛИ` | `OR`.
    ![image](https://github.com/user-attachments/assets/640dae8c-16df-4f57-b3bb-6a74d9666d02)
  - `Perceptron` работает корректно, обучился с 3 эпох
  - ![image](https://github.com/user-attachments/assets/0f6e8220-1f51-499b-afbc-a497b8a32a30)


  ### AND
  - Настроил `TrainingSet` на обучение вычисления логического `И` | `AND`.
    ![image](https://github.com/user-attachments/assets/80345f6f-f971-4d17-80db-88d25e309e76)
  - `Perceptron` работает корректно, обучился с 7 эпох
  - ![image](https://github.com/user-attachments/assets/0b113ffb-2582-4a04-a8e3-5784b88d589b)


  ### NAND
  - Настроил `TrainingSet` на обучение вычисления логического `НЕ И` | `NAND`. Тоже самое, что `AND`, только с инвертированным выводом.
  - `Perceptron` работает корректно, обучился с 9 эпох
  - ![image](https://github.com/user-attachments/assets/d65be715-330c-4515-9a83-7cc326a6a71f)

  ### XOR
  - Поскольку `Perceptron` работает только линейно, то он не может справиться с `XOR`, так как это нелинейная функция.
  - `Perceptron` работает некорректно.
  - ![image](https://github.com/user-attachments/assets/d608ad48-15ae-4005-8b0d-557a9a44d71f)
    


## Задание 2
### Построить графики зависимости количества эпох от ошибки  обучения. Указать от чего зависит необходимое количество эпох обучения.

Ход работы:
- Построил графики зависимости количества эпох от ошибок обучения
  ### OR
  <img width="325" alt="or" src="https://github.com/user-attachments/assets/ec789003-5a3a-44da-9416-f98eb6da77b4" />

  ### AND
  <img width="359" alt="nand" src="https://github.com/user-attachments/assets/e41ceda5-d996-4b01-be05-065e9da4e405" />

  ### NAND
  <img width="359" alt="and" src="https://github.com/user-attachments/assets/3dae64c9-1f78-4fe6-a06e-b97a55904e32" />

  ### XOR
  <img width="362" alt="xor" src="https://github.com/user-attachments/assets/71fe5fac-6296-4cc2-83a5-24a596173b7e" />

  - Необходимое количество эпох для обучения перцептрона зависит от сложности функции (OR<AND/NAND<XOR). 

## Задание 3
### Построить визуальную модель работы перцептрона на сцене Unity.

## Выводы
- В ходе данной лабораторной работы я изучил работу перцептрона, реализовав в Unity перцептрон, которого обучил производить корректные логические операции OR, AND и NAND. 
- Изучил почему перцептрон работает некорректно с операцией XOR.
- Построил графики зависимости количества эпох от ошибок обучения и проанализировал их.

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
