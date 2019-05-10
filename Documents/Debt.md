## Технический долг

### Обзор всего кода в целом
- По причине построения приложения по микросервисной архитектуре, использования фреймворков Spring и Angular, код является структурированным и понятным. Выявление места возникновения ошибок не составляет труда, особенно с использованием стороннего ПО для осуществления HTTP запросов.
- Ввиду сдвинутых сроков третьего спринта к его концу не был до конца реализован механизм отображения статистики платежей пользователя. Не реализовано покрытие автотестами.
- Отсутствие достаточных практических навыков использования фреймворка Angular не позволило создать "front-end" составляющую приложения легкочитабельной и простой для понимания новыми членами команды.

### Имеющийся технический долг
Краткий список проблем выглядит следующим образом:
- Низкое покрытие тестами;
- Не реализован сбор статистики платежей пользователя;
- Улучшение качества кода "front-end" составляющей.

### Почему так получилось и как это можно решить?
- Низкое покрытие кода тестами обусловлено необходимостью реализации большого количества end-to-end решений для демонстрации. Использование фреймворка Spring позволяет избежать многих ошибок за счет декомпозиции логики приложения, что ведет к отсутствию необходимости в автотестах.

- Так получилось по причине неожиданного сдвига границ третьего спринта и недостаточно продуманного распределения задач по членам команды. Планируется доделать этот функционал до финальной демонстрации.

- Низкое качество кода "front-end" составляющей обусловлено недостатком опыта использования фреймворка Angular. Планируется провести рефакторинг.

### Cравнение технического долга и еще нереализованных возможностей приложения
- Нереализованные возможности приложения: сбор статистики платежей пользователя ("front-end" составляющая).
- Технический долг: покрытие тестами, рефакторинг "front-end" составляющей.
На данный момент объем трудозатрат на исполнение технического долга значительно меньше соответствующего объема трудозатрат на реализацию запланированного функционала приложения.

### Тикеты на устранение технического долга
- рефакторинг - (ERT-18) - 4 story points
- unit-test - (ERT-17) - 7 story points
- сбор статистики - (ERT-87) - 10 story points