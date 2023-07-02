# minly-backend (backend on Golang)

minly - проект для сокращения ссылок с открытым исходным кодом. Бекенд minly имеет два хендлера GET-запросов: getLink, getResult.

## Стек
Echo, mongo-driver

## Доступные запросы
### getLink (result string)

Возвращает изначальную ссылку по идентификатору.

### getResult (initial string, only_result bool)

Возвращает результат сокращения ссылки в виде JSON-объекта. 

# JSON-объект

хранит в себе
* initial - изначальная ссылка
* result - идентификатор из пяти символов
* counter - количество раз, когда запрашивали сокращённую ссылку

