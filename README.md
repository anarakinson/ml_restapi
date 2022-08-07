
Предполагаемая структура сервиса:

- main.py — приложение Flask, которое взаимодействует с клиентом и возвращает предсказание модели
- model.py — файл с функциями загрузки моделей
- models/ — папка с сохранёнными моделями
- logs/ — папка с логами

Доступ к API должен осуществляться по следующему URL:
`http://[hostname]/iris/api/v1.0/getpred`
В качестве примера запроса можно использовать:
`http://[hostname]/iris/api/v1.0/getpred?sepal_length=5.1&sepal_width=3.5&petal_length=1.4&petal_width=0.2`

также должны присутствовать:
`http://[hostname]/iris/api/v1.0/status/`
- для проверки статуса выполнения запроса к сервису
`http://[hostname]/iris/api/v1.0/result/`
- для получения результаты работы модели.
