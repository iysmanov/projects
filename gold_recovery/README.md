Подготовьте прототип модели машинного обучения для «Цифры». Компания разрабатывает решения для эффективной работы промышленных предприятий.
Модель должна предсказать коэффициент восстановления золота из золотосодержащей руды. Используйте данные с параметрами добычи и очистки. 
Модель поможет оптимизировать производство, чтобы не запускать предприятие с убыточными характеристиками.

Вам нужно:

1. Подготовить данные;
2. Провести исследовательский анализ данных;
3. Построить и обучить модель.

# Описание данных

Технологический процесс:
<br /> Rougher feed — исходное сырье
<br />Rougher additions (или reagent additions) — флотационные реагенты: Xanthate, Sulphate, Depressant 
- Xanthate - ксантогенат (промотер, или активатор флотации);
- Sulphate — сульфат (на данном производстве сульфид натрия);
- Depressant — депрессант (силикат натрия).

<br />Rougher process (англ. «грубый процесс») — флотация
<br />Rougher tails — отвальные хвосты
<br />Float banks — флотационная установка
<br />Cleaner process — очистка
<br />Rougher Au — черновой концентрат золота
<br />Final Au — финальный концентрат золота

<br />Параметры этапов:
- air amount — объём воздуха
- fluid levels — уровень жидкости
- feed size — размер гранул сырья
- feed rate — скорость подачи

# Наименование признаков

Наименование признаков должно быть такое:
<br /> [этап].[тип_параметра].[название_параметра]
<br /> Пример: rougher.input.feed_ag
<br /> Возможные значения для блока [этап]:
- rougher — флотация
- primary_cleaner — первичная очистка
- secondary_cleaner — вторичная очистка
- final — финальные характеристики

<br /> Возможные значения для блока [тип_параметра]:
- input — параметры сырья
- output — параметры продукта
- state — параметры, характеризующие текущее состояние этапа
- calculation — расчётные характеристики