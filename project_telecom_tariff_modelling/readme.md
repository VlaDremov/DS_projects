## Данные

В распоряжении данные о поведении клиентов, которые уже перешли на тарифы оператора связи. 
Нужно построить модель для задачи классификации, которая выберет подходящий тариф. 
Предобработка данных не понадобится — она уже сделана.
Постройте модель с максимально большим значением accuracy. 

В качестве исходных данных получена 1 таблица с информацией о том, в каком объеме клиенты пользуются услугами оператора связи и какой у них тариф.
Описание полей:

Поля таблиц:
- сalls — количество звонков,
- minutes — суммарная длительность звонков в минутах,
- messages — количество sms-сообщений,
- mb_used — израсходованный интернет-трафик в Мб,
- is_ultra — каким тарифом пользовался в течение месяца («Ультра» — 1, «Смарт» — 0).

## Задача

На основе данных клиентов оператора сотовой связи проанализировать поведение клиентов и произвести поиск оптимального тарифа


## Используемые библиотеки
*pandas*, *sklearn*, *numpy*

