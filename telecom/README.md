# **Телеком**

Оператор связи «Ниединогоразрыва.ком» хочет научиться прогнозировать отток клиентов. 
Если выяснится, что пользователь планирует уйти, ему будут предложены промокоды и специальные условия.
Команда оператора собрала персональные данные о некоторых клиентах, информацию об их тарифах и договорах. 
Информация о договорах актуальна на 1 февраля 2020.

## *Описание услуг*

Оператор предоставляет два основных типа услуг:

 - Стационарную телефонную связь. Возможно подключение телефонного аппарата к нескольким линиям одновременно.
 - Интернет. Подключение может быть двух типов: через телефонную линию (DSL) или оптоволоконный кабель (Fiber optic).
Также доступны такие услуги.

За услуги клиенты могут платить каждый месяц или заключить договор на 1–2 года. 
Доступны различные способы расчёта и возможность получения электронного чека.

## Цель исследования:

Построить модель классификации для прогнозирования оттока клиентов с максимально большим значением $Roc-auc$(по крайней мере до 0.86) 
Проверить на тестовой выборке. Дополнительно сравнивнить её значение с $F_1$-мерой.

## Ход исследования:

 - загрузка и предварительная обработка данных - описание данных, проверка пропусков, дубликатов, заголовков колонок с признаками, 
   подсчет коэфф.корреляции в phik, поиск аномалий
 - разбиение данных на тестовую и тренировочную выборки в соотношении 1:3; кодирование и масштабирование признаков
 - создание моделей для решения задачи бинарной классификации, подбор параметров и подсчет метрик; построение *roc_curve*
 - тестирование лучшей модели и интерпретация результатов.
