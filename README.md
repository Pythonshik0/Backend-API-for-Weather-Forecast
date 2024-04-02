# Серверный API для прогнозирования погоды

# Weather API с Flask
В этом проекте реализован простой погодный API с использованием Flask,
позволяющий пользователям получать текущую информацию о погоде для нескольких местоположений.
Данные о погоде извлекаются из OpenWeatherMap API.

### Предварительные условия
- Python
- Flask
- Библиотека запросов

### Краткая процедура
1. Установите необходимые библиотеки.
2. Получите свой API-ключ OpenWeatherMap.
3. Запустите приложение.
4. Откройте Postman и создайте новый запрос на `http://127.0.0.1:5000/weather` с помощью метода `GET`.
5. Добавьте параметр запроса `местоположение`, указав в нем город и штат (например, "Бангалор, Калифорния").
6. Отправьте запрос и проверьте результат.
7. ПРИМЕЧАНИЕ: Вы можете проверить точность полученных данных о погоде с помощью "OpenWeatherMap".

## Подробное объяснение
1. Запустите скрипт на python в VSCode
2. В терминале вы можете увидеть базовый URL-адрес `http://127.0.0.1:5000`. Когда вы нажмете на этот URL-адрес, вы увидите сообщение об ошибке 404.
3. Теперь перейдите в рабочее пространство Postman и задайте тип запроса "ПОЛУЧИТЬ".
4. Введите URL-адрес конечной точки вашего Flask API, т.е. `http://127.0.0.1:5000/weather?`.
5. Перейдите на вкладку "Параметры". В столбце "Ключ" введите "местоположение". В столбце "Значение" введите город и штат, для которых вы хотите получить информацию о погоде.
6. Нажмите кнопку "Отправить", чтобы отправить запрос.
7. Теперь вернитесь к базовому URL-адресу, чтобы получить данные о погоде, вы должны добавить базовый URL-адрес к конечной точке api, т.е. (например: `http://127.0.0.1:5000/weather?location=city,state` (`http://127.0.0.1:5000/weather?location=Bengaluru, Karnataka&location=Mysore, Karnataka`).
8. Теперь вы можете просмотреть файл json.

## Screenshots 
![Screenshot 2023-11-24 183521](https://github.com/Sanjana-np/Backend-API-for-Weather-Forecast/assets/136239239/4a0cae74-c58f-4a6a-bdca-a6cde747bdca)
![Screenshot 2023-11-24 184828](https://github.com/Sanjana-np/Backend-API-for-Weather-Forecast/assets/136239239/8b2f850b-d2cd-4cca-a81a-7d05767e34d5)
![Screenshot 2023-11-24 185009](https://github.com/Sanjana-np/Backend-API-for-Weather-Forecast/assets/136239239/83dc2f82-4e2e-4d93-9f3e-eb878c0b4bc3)
![Screenshot 2023-11-24 185041](https://github.com/Sanjana-np/Backend-API-for-Weather-Forecast/assets/136239239/9d7c650a-1f4c-44bb-bc31-342bf3569c74)

## Additionals 
1. This python script accepts multiple query parameters. The code includes the ability to retrieve weather information for multiple locations through the `/weather` endpoint. 
2. The code includes try-except blocks to catch and handle exceptions that may occur during API requests or data processing.
3. Appropriate status codes are returned in the API responses, such as `400 for bad requests`, `200 for response` and `500 for internal server errors`.

## ## Дополнительно
1. Этот скрипт на python принимает несколько параметров запроса. Код включает в себя возможность получения информации о погоде для нескольких местоположений через конечную точку `/weather`.
2. Код включает в себя блоки try-except для перехвата и обработки исключений, которые могут возникать во время запросов API или обработки данных.
3. В ответах API возвращаются соответствующие коды состояния, такие как "400 для неверных запросов", "200 для ответа" и "500 для внутренних ошибок сервера`.







