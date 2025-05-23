# mkrf_movies
Исследование данных о российском кинопрокате

Цель исследования
Изучение рынка российского кинопроката и выявление текущих тренды. Анализ восстребованности у зрителей фильмов, получивших государственную поддержку.

Входные данные

Данные, опубликованные на портале открытых данных Министерства культуры. Набор данных содержит информацию о прокатных удостоверениях, сборах и государственной поддержке фильмов, а также информацию с сайта КиноПоиск.

Пути к файлам: /datasets/mkrf_movies.csv — данные о прокатных удостоверениях.

/datasets/mkrf_shows.csv — данные о прокате в российских кинотеатрах.

Таблица mkrf_movies содержит информацию из реестра прокатных удостоверений. У одного фильма может быть несколько прокатных удостоверений.

title — название фильма;

puNumber — номер прокатного удостоверения;

show_start_date — дата премьеры фильма;

type — тип фильма;

film_studio — студия-производитель;

production_country — страна-производитель;

director — режиссёр;

producer — продюсер;

age_restriction — возрастная категория;

refundable_support — объём возвратных средств государственной поддержки;

nonrefundable_support — объём невозвратных средств государственной поддержки;

financing_source — источник государственного финансирования;

budget — общий бюджет фильма;

ratings — рейтинг фильма на КиноПоиске;

genres — жанр фильма.

Таблица mkrf_shows содержит сведения о показах фильмов в российских кинотеатрах.

puNumber — номер прокатного удостоверения;

box_office — сборы в рублях.

Ход исследования

Обзор данных:

- Импортирование необходимых библиотек.
- Чтение файлов с данными.
- Общий обзор информации.
- Объеденение данных в один датафрейм

Предобработка данных:
- Приведение именования столбоц к общей стилистике.
- Проверка на пропущенные значения и их заполнение или удаление.
- Удаление дубликатов.
- Преобразование типов данных (например, приведение дат к единому формату).
- Обработка выбросов и аномалий (например, нереально высокие или низкие цены).
- Создание новых признаков.

Исследовательский анализ данных (EDA):
- Анализ количества выщедших в прокат фильмов Российского и зарубежного производства.
- Анализ сборов по годам
- Анализ кассовых сборов и фильмов по годам
- Анализ средней и медианной суммы для каждого года
- Исследование фильмов с господдержкой
- Общий анализ господдержки
- Анализ окупаемости фильмов с господдержкой
- Анализ рейтинга фильмов с господдержкой
- Анализ распределения по жанрам среди фильмов с господдержкой

Формирование выводов:
- Общий вывод по исследованию российского кинопроката и господдержки фильмов (2010–2019)
