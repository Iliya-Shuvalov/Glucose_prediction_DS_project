# Прогнозирование уровня глюкозы в крови животного при заболевании сахарным диабетом с иcпользованием методов машинного обучения 
(Predicting blood glucose levels in an animal with diabetes mellitus using machine learning methods)

## Постановка задачи

Построение модели машинного обучения, позволяющей осуществить проверку схемы заместительной инсулинотерапии, применяемой для 
регулирования уровня глюкозы в крови животного с заболеванием сахарным диабетом. прогноз значения глюкозы в крови должен 
осуществляться на следующие 24 часа при заданном объёме вводимого инсулина и времени инъекции. Необходимо предусмотреть
возможность изменения интервала прогнозирования в случае изменения схемы заместительной инсулинотерапии. 

Средняя абсолютная ошибка (MAE) прогноза модели на интервале 24 часа должна составлять менее 5 ммоль/л.

(Building a machine learning model that allows you to test the scheme of insulin replacement therapy used for
regulation of blood glucose levels in an animal with diabetes mellitus. blood glucose prediction
carried out for the next 24 hours at a given volume of insulin administered and injection time. It is necessary to provide
the possibility of changing the prediction interval in case of a change in the regimen of insulin replacement therapy.
The mean absolute error (MAE) of the model prediction over a 24-hour interval should be less than 5 mmol/L.)

## Описание данных

данные находятся в таблице insulin_31_05_23.xlsx. В таблицу занесены дата и время измерений - столбец  'injection_datetime',
уровень глюкозы (ммоль/л.) - столбец 'glucose_level' и объём введеного инсулина (в ед.) - столбец 'insulin_dose'.

(the data is in the insulin_31_05_23.xlsx table. The table contains the date and time of measurements - column 'injection_datetime',
glucose level (mmol/l.) - column 'glucose_level' and volume of injected insulin (in units) - column 'insulin_dose'.)

## Используемые инструменты

`pandas` `numpy` `seaborn` `matplotlib` `sklearn` `adfuller` `tsaplots`

### Модели

`Ridge`

### Метрики

`mean_absolute_error`
