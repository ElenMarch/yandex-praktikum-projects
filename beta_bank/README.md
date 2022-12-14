# *Отток клиентов*

Из «Бета-Банка» ежемесячно стали уходить клиенты. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых. 
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. 
Предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

## Цель исследования: 

Построить модель с предельно большим значением F1-меры(не менее 0.59).
Проверим F1-меру на тестовой выборке, дополнительно рассмотрим AUC-ROC в сравнении с F1-мерой.

## Ход исследования:

 - подготовка данных
 - исследование задачи, обучение моделей классификации
 - борьба с дисбалансом
 - тестирование модели
 
Источник данных: https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling
