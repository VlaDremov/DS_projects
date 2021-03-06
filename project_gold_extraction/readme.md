## Данные

Компания разрабатывает решения для эффективной работы золотодобывающей отрасли.
Построена модель, предсказывающая коэффициент восстановления золота из золотосодержащей руды. Проанализированы данные с параметрами добычи и очистки.
Построена и обучена модель, помогающая оптимизировать производство, чтобы не запускать предприятие с убыточными характеристиками.

Нужно:

1. Подготовить данные;
2. Провести исследовательский анализ данных;
3. Построить и обучить модель.

**Технологический процесс**

-   _Rougher feed_  — исходное сырье
-   _Rougher additions_  (или  _reagent additions_) — флотационные реагенты:  _Xanthate, Sulphate, Depressant_
    -   _Xanthate_  _**_— ксантогенат (промотер, или активатор флотации);
    -   _Sulphate_  — сульфат (на данном производстве сульфид натрия);
    -   _Depressant_  — депрессант (силикат натрия).
-   _Rougher process_  (англ. «грубый процесс») — флотация
-   _Rougher tails_  — отвальные хвосты
-   _Float banks_  — флотационная установка
-   _Cleaner process_  — очистка
-   _Rougher Au_  — черновой концентрат золота
-   _Final Au_  — финальный концентрат золота

**Параметры этапов**

-   _air amount_  — объём воздуха
-   _fluid levels_  — уровень жидкости
-   _feed size_  — размер гранул сырья
-   _feed rate —_  скорость подачи

## **Наименование признаков**

Наименование признаков должно быть такое:

`[этап].[тип_параметра].[название_параметра]`

Пример:  `rougher.input.feed_ag`

Возможные значения для блока  `[этап]`:

-   _rougher —_  флотация
-   _primary_cleaner_  — первичная очистка
-   _secondary_cleaner_  — вторичная очистка
-   _final_  — финальные характеристики

Возможные значения для блока  `[тип_параметра]`:

-   _input_  — параметры сырья
-   _output_  — параметры продукта
-   _state_  — параметры, характеризующие текущее состояние этапа
-   _calculation —_  расчётные характеристики

## Задача

Разработка модели, предсказывающей коэффициент восстановления золота из золотосодержащей руды.

## Используемые библиотеки
*pandas*, *matplotlib*, *numpy*, *sklearn*, *catboost*
