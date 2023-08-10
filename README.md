# **Портфолио: аналитик данных**

## **Обо мне**

Привет! Меня зовут Татьяна, я начинающий аналитик данных. На протяжении всей своей 17-ти летней трудовой деятельности занималась сбором и изучением данных в следующих различных областях:
- Руководитель проекта: аренда инструмента (самозанятый);
- Финансовый директор в ООО "Агрофирма "Прииртышская";
- Заместитель начальника Операционного отдела в Филиале АО "ГЕНБАНК" в г. Омске;
- Начальник Отдела валютных операций в ФКБ «ЮНИАСТРУМ БАНК» в Омске и др.

Люблю находить закономерности и делать логические выводы на базе проведенного анализа. Умею мыслить логически, чтобы структурировать полученную информацию и находить закономерности в потоках данных.

В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практик.

## **Навыки и технологии:**
- Инструменты анализа данных: SQL, Excel;
- Языки программирования и библиотеки: Python, Pandas, math;
- Системы управления базами данных: MySQL, PostgreSQL;
- Средства визуализации данных: PowerBi, Metabase.

  
## Проекты

### ***Проект 1: Калькулятор юнит-экономики онлайн-школы.***

Что нужно было сделать:

Задача №1. Настроить в калькуляторе юнит-экономики сценарий, при котором планы маркетинга будут увеличены на 12%.

Задача №2. Составить план найма преподавателей и сценарий, при котором Пропускная способность Преподавателей увеличится на 15%, а Retention Преподавателей упадёт на 2%. Составить новый план найма с ограничением: за месяц нельзя нанять более 70 преподавателей.

Как решала: 
1) Создаю сводные таблицы, на основе которых расчитываю следующие показатели: Средний Retention, Lifetime (месяцы), Средняя интенсивность, Lifetime (уроки), Средняя цена урока, LTR, CAC, ЗП Учителя на 1 урок, Fixed costs на 1 урок. Расчитываю показатели юнит-экономики : CAC, ЗП Учителя на 1 урок, Fixed costs на 1 урок, Маржа. На основании полученных данных строю калькулятор юнит-экономики с учётом корректровки планов маркетинга.
2) Строю калькулятор Найма преподавателей с возможность изменять входных параметры: Пропускную способность Преподавателей и Retention Преподавателей. Составляю сценарий, при котором Пропускная способность П увеличится на 15%, а Retention П упадёт на 2%. С помощью функции "Поиск решений" составила новый план найма с ограничением: за месяц нельзя нанять более 70 преподавателей.

Ссылка на проект: 
[Проект 1](https://github.com/Totyana/Portfolio-Data-Analyst/tree/main/Project_1).


Итоги:

Итог №1. Лист с калькулятором + расчёт количества студентов на 04.2022.

Итог №2. План по найму - с количеством новых преподавателей по месяцам за период с 05.2021 по 04.2022.
<p><br>
  
### ***Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра.***

Что нужно было сделать:

Задача №1. Просчитать юнит-экономику продукта и предложить сценарий по настройке параметров для выхода на 25-ти процентную маржинальность.

Задача №2. Визуализировать какие пользователи, где и в каком объеме смотрят фильмы на платформе.

Как решала: 
1) Определила, что является юнитом в экономике онлайн-кинотеатра. Расчитала юнит-экономику продукта и предложила сценарий по настройке параметров для выхода на 25%-ную маржинальность. Собрала визуализацию основных бизнес-показателей.
2) Исследовала данные о пользователях онлайн-кинотеатра и их поведении.

Ссылка на проект:
[Проект 2](https://github.com/Totyana/Portfolio-Data-Analyst/tree/main/Project_2).

Итоги:

Итог №1. Построен Лист с калькулятором юнит-экономики. 
Для того, чтобы выйти на маржинальность 25% предлагаю следующий сценарий: Retention увеличить на 15%, Price юнита увеличить на 25%,  Базовую цену подписки установить 400 руб., CAC (средний) уменьшить на 11,2%.

Итог №2. Создана визуализация следующих данных: 
- ТОП-5 самых популярных фильмов;
- Активность пользователей (сделан вывод: пользователи больше всего смотрят фильмов в субботу и воскресенье, а самая низкая активность пользователей приходится на вторник);
- Распределение подписчиков по часовым поясам (сделан вывод: самое большое количество подписчиков из региона с часовым поясом UTC+1, а самое маленькое количество подписчиков из регионов с часовым поясом UTC-2 и UTC-9);
- Активность пользователей по часам (сделан вывод: пик активности пользователей расположен в диапазоне 18-20 часов, а спад активности пользователей зафиксирован в диапазона 4-7 часов).
<p><br>

### ***Проект 3: Когортный анализ онлайн-кинотеатра с помощью SQL.***

Что нужно было сделать:

Задача №1. Построить распределение выплаченных клиентами денег по месяцам и получилось три разных скользящих средних (по сумме денег по месяцам) (SQL-запрос).

Задача №2. Построить графики скользящего среднего (по сумме денег по месяцам).

Как решала: 
1) Построила распределение выплаченных клиентами денег (amt_payment) по месяцам поля date_purchase (SQL-запрос). Дополнила SQL-запрос так, чтобы получилось три разных скользящих средних (по сумме денег по месяцам):
- MA(3) — скользящее среднее, принимающее текущее значение и два предыдущих;
- MA(7) — скользящее среднее, принимающее текущее значение и шесть предыдущих;
- MA_2side(5) — двустороннее скользящее среднее, принимающее текущее значение, два предыдущих и два следующих.
2) Перенесла результаты в Excel и построила графики скользящего среднего.

Ссылка на проект:
[Проект 3](https://github.com/Totyana/Portfolio-Data-Analyst/tree/main/Project_3).

Итоги:

Итог №1. Составлен SQL-запрос и получены данные о выплаченных клиентами денег по месяцам и данные о трёх разных скользящих средних.

Итог №2. Получены графики скользящего среднего (по сумме денег по месяцам).
<p><br>

### ***Проект 4: Построение витрины для модели машинного обучения в банке с помощью SQL.***

Что нужно было сделать: 

Задача №1. Составить витрину для модели машинного обучения в соотвествии с требованиями отдела машинного обучения в банке.

Как решала:
Взяла две таблицы и написала скрипт, который сделал витрину со следующими полями:
- Внутренний идентификатор клиент;
- Название города;
- Числовой признак, который принимает значение 1 для мужчин и 0 для женщин;
- Возраст;
- Числовая переменная, которая показывает, в первый ли раз клиент обратился к нам за кредитом;
- Числовой признак, который принимает значение 1 при наличии мобильного телефона и 0 при его отсутствии;
- Числовая переменная, которая показывает, активен ли клиент;
- Номер клиентского сегмента;
- Размер выданного кредита;
- Дата выдачи кредита;
- Тип выданного кредита;
- Суммарный объем кредитов, выданных в этом городе;
- Доля данного кредита среди всех кредитов, выданных в этом городе и другие.

Ссылка на проект:
[Проект 4](https://github.com/Totyana/Portfolio-Data-Analyst/tree/main/Project_4).

Итог: создана витрина для модели машинного обучения.
<p><br>

### ***Проект 5: Моделирование изменения балансов студентов с помощью SQL.***

Что нужно было сделать:

Задача №1. Соберите вопросы к дата-инженерам и владельцам таблицы.

Задача №2. Соберите выводы из визуализации (линейной диаграммы) получившегося результата. 

Как решала:
1) Написала SQL-запрос, который собирает данные о балансах студентов за каждый прожитый ими день.
2) Изучала изменения балансов студентов (на примере топ-1000 строк), собранных из CTE. На основании этих данных выдвинула гипотезы.
3) Создала визуализацию (линейную диаграмму) итогового результата на ее основании выбдинула гипотезы.

Ссылка на проект:
[Проект 5](https://github.com/Totyana/Portfolio-Data-Analyst/tree/main/Project_5).

Итоги:

Итог №1. Написан SQL-запрос. Сформулированы следующие вопросы для дата-инженеров и владельцам таблицы:
- Нет ли шибок в количестве пройденных уроков в день? У некоторых студентов списывается по 4/3 урока в день. В среднем один студент проходит по 1/2 урока в день;
- Почему у некоторых студентов появляется отрицательный баланс уроков?;
- Почему в таблице payments есть успешные транзакции, но при этом нет id транзакции?

Итог №2.  Написан SQL-запрос. Создан график балансов студентов. Выдвинуты следующие гипотезы:
- Студенты тратят (проходят) уроки медленнее, чем покупают;
- В конце 2016 года на балансе студентов остается 4534 урока. Соответственно эти уроки в 2017 году станут для школы пассивом, т.к. студент заплатил за них в 2016 году, а расходы на учителей школа понесёт в 2017 году. Это может отрицательно повлиять на финансовые показатели 2017 года и на загруженность учителей;
- Пик покупок уроков возможно связан с сезонностью (студенты начинают учиться осенью). Возможно, зависит от зарплаты/аванса студентов, т.к. некоторые пики покупок студентов приходятся на конец и начало месяца.Возможно, некоторые пики покупок уроков происходили в единоразовые маркетинговые акции/распродажи;
- Заметно, что график списания уроков идёт циклом. Это говорит о том, что студенты чаще всего проходят уроки в будние дни, чем в выходные дни.
