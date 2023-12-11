# Приборная панель

### Тест стрелок при включении зажигания 
При включении зажигания стрелки тахометра и спидометра совершают ход от минимального до максимального положения.   
Функционал никакой, зато смотрится эффектно!   
``` yaml
Блок 17 → Адаптация: 
канал «indicator_celebration» → выбираем «active» → выполнить 
```
 
### Показ свободного месте в бензобаке в литрах 
Остаток места в баке – приблизительное значение литров, которые можно залить в бак. Шаг шкалы – 5 литров.   
При полностью заправленном баке отображается «---». Показания приблизительные и могут варьироваться ±10 л.
``` yaml
Блок 17 → Адаптация: 
канал «Volume to be replenished» → выставить значение «yes» → выполнить 
```
 
### Отключение звукового сигнала и индикации о не пристегнутом ремне 
По умолчанию на некоторых автомобилях включен контроль ремня водителя и переднего пассажира.   
Если кто любит кататься без ремня безопасности, эту функцию можно отключить. 
``` yaml
Блок 17 → Кодирование → Длинное кодирование:
Байт 1 – Бит 1: Деактивировать 
```
 
### Корректировка показаний спидометра 
В соответствии с нормами безопасности показания спидометра слегка завышены относительно реальной скорости.   
Для разных автомобилей предусмотрены различные уровни завышения показаний.   
Число импульсов от Skoda Octavia (01) завышает показание при 100 км/ч ≈ на 8 км/ч, от Skoda Fabia (02) ≈ на 15 км/ч.   
Самое точное показание на колёсах размерности 215/65 R16 при установке числа импульсов от VW Golf (07).   
``` yaml
Блок 17 → Кодирование → Длинное кодирование:
Байт 0 – Бит 0-3 → 07 Distance Impulse Number 7 
```
 
### Корректировка показаний уровня топлива 
Датчик уровня топлива в баке имеет погрешность, из-за чего неточность в показаниях может достигать ±10 л. 
``` yaml
Блок 17 → Адаптация: 
канал "Display correction of fuel gauge" → Подбираем значение (от -10 до 10) → выполнить 
```

Чтобы скорректировать показания, нужно точно знать, сколько бензина в баке или дождаться загорания лампочки.  
Ёмкость бака – 64 л, цена деления – 4 л. Контрольная лампа низкого уровня топлива загорается при остатке 7 л в баке. 
 
 