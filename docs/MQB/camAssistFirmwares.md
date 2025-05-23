---
hide:
  - toc
---

# Прошивки для камеры ассистентов

Для полноценной работы камеры ассистентов нужна правильная прошивка и параметрия к ней.  
Камеры могут быть 3 вариантов:  

* 5Q0... - MFK 1.0 (Lane Assist, Sign Assist, DLA)  
* 3Q0/3QD... - MFK 2.0 (Lane Assist, Sign Assist, Traffic Jam Assist, DLA)  
* 2Q0... - MFK 3.0 (Lane Assist, Sign Assist, Traffic Jam Assist, Pedestrian Assist, DLA)  

Параметрии для прошивок L и H с увеличенным временем предупреждения (60с) для разных машин можно найти на [https://mibsolution.one](https://mibsolution.one/#/1/9/Datasets/MQB/A5/60+%20Mod)

## Прошивки для камер вида MFK3

| ID оборудования              |                         Прошивка                         |                               Параметрия<br/>(ODIS XML)                               | Примечания |
|------------------------------|:--------------------------------------------------------:|:-------------------------------------------------------------------------------------:|:----------:|
| FL_2Q0980653_1400_2Q0980653D | [(Скачать)](../firmwares/FL_2Q0980653D_1400_MEAPP_S.pdx) | [(Скачать для Škoda)](../parameters/A5_2Q0980653D_1400_VHL125933Q1A_MFK_3G0_0831.xml) |            |

## Прошивки для камер вида MFK2

!!! warning "Важно!"
    Порядок обновления должен быть следующим: G → H → L → T → Q → R → S → T  
    Изменение этого порядка в обратном порядке повредит вашу камеру

Поколение 4:  

| ID оборудования              |                    Прошивка                     |              Параметрия<br/>(ODIS XML)               |                                  Примечания                                   |
|------------------------------|:-----------------------------------------------:|:----------------------------------------------------:|:-----------------------------------------------------------------------------:|
| FL_3Q0980654_0920_3Q0980654S | [(Скачать)](../firmwares/FL_3Q0980654_0920.frf) | [(Скачать)](../parameters/A5_3Q0980654S_BW2_STA.xml) | Не рекомендуется для Tiguan 2G.<br/>Существуют проблемы с удержанием в полосе |
| FL_3Q0980654_0460_3Q0980654R |                                                 |                                                      |                                                                               |
| FL_3Q0980654_0881_3Q0980654Q |                                                 |                                                      |                                                                               |
| FL_3Q0980654_0451_3Q0980654M |                                                 |                                                      |                                                                               |

Поколение 3:  

| ID оборудования              |                    Прошивка                     |                           Параметрия<br/>(ODIS XML)                            |                     Примечания                      |
|------------------------------|:-----------------------------------------------:|:------------------------------------------------------------------------------:|:---------------------------------------------------:|
| FL_3Q0980654_0611_3QD980654T |                                                 |                                                                                | Прошивка для Tiguan 2G от модельного ряда 2020 года |
| FL_3Q0980654_0610_3QD980654L | [(Скачать)](../firmwares/FL_3Q0980654_0610.frf) | [(Скачать для VW Tiguan (60s)](../parameters/A5_3Q0980654L_wTJ_Tiguan_60+.xml) |                                                     |
| FL_3QD980654_1611_3QD980654A | [(Скачать)](../firmwares/FL_3QD980654_1611.odx) |    [(Скачать для Škoda и Seat)](../parameters/A5_3Q0980654L_SEAT_Leon.xml)     |                                                     |

Поколение 2:  

| ID оборудования              |                    Прошивка                     |                           Параметрия<br/>(ODIS XML)                            | Примечания |
|------------------------------|:-----------------------------------------------:|:------------------------------------------------------------------------------:|:----------:|
| FL_3Q0980654_0272_3QD980654H | [(Скачать)](../firmwares/FL_3Q0980654_0272.frf) | [(Скачать для VW Tiguan (60s)](../parameters/A5_3Q0980654H_wTJ_Tiguan_60+.xml) |            |
| FL_3QD980654_1272_3QD980654  |                                                 |          [(Скачать)](../parameters/A5_3Q0980654H_wTJ_Tiguan_60+.xml)           |            |
| FL_3Q0980654_0231_3QD980654G | [(Скачать)](../firmwares/FL_3Q0980654_0231.frf) |                                                                                |            |
| FL_3Q0980654_0220_3QD980654F |                                                 |                                                                                |            |

Поколение 1:  

| ID оборудования              | Прошивка | Параметрия<br/>(ODIS XML) | Примечания |
|------------------------------|:--------:|:-------------------------:|:----------:|
| FL_3Q0980654_0024_3Q0980654D |          |                           |            |
| FL_3Q0980654_0010_3Q0980654C |          |                           |            |
