# Вопросы для разработчиков Python

* [Вопросы по soft skills](/questions/common/softskills.md)
* [Вопросы по алгоритмам](/questions/common/algorithms.md)
* [Вопросы по базам данных](/common/databases.md)
* [Вопросы по сетям](/common/networks.md)
* [вопросы по методологиям разработки](/common/metodologies.md)

## Junior

### Общие вопросы

1. Почему ты решил стать бэкенд-разработчиком, чем тебя привлекает профессия?

### Python

1. Какие типы данных существуют в Python?
1. Области видимости в Python. Как работают?
1. Методы работы со списками, какие существуют?
1. Как устроены хеш-мапы в Python?
1. В чем разница между операторами `is` и `==`?
1. Какие циклы существуют в Python?
1. Что такое контекстный менеджер? Для чего он используется?
1. Что такое магические методы в Python? Как они работают?
1. В чем разница между приватными и защищенными методами?
1. Различия между `staticmethod` и `classmethod`.
1. Что такое GIL? Как он влияет на многозадачность в Python?
1. Что может быть ключом словаря, а что не может? Почему?
1. Как устроено наследование в Python? Как работает множественное наследование?
1. Что такое ленивые вычисления в Python?
1. В чем разница между Flask и FastAPI?
1. Что такое сериализация? Где и зачем она используется?

### Базы данных

1. Какие бывают типы баз данных? В чем их отличия?
1. В чем разница между `JOIN` и `UNION`?
1. В чем различия между `UNION` и `UNION ALL`?
1. Какие требования предъявляются к оператору `UNION`?
1. В чем разница между `HAVING` и `WHERE`?
1. Что такое индексы в базах данных? Какие плюсы и минусы у их использования?
1. Что такое SQL-инъекции? Как их предотвратить?
1. Что такое транзакции? Как они работают?
1. Какие ORM знаешь и какие использовал? Какие плюсы и минусы можешь выделить?
1. Если соединяем несколько таблиц БД с помощью `INNER JOIN`, есть ли разница в оптимизации, в каком порядке соединяем таблицы?

### Сети

1. Какие бывают протоколы передачи данных?
1. В чем разница между HTTP и HTTPS?
1. В чем разница между UDP и TCP?
1. Какие методы HTTP существуют? Как они различаются?
1. Что такое JWT токен?
1. Что такое REST API и как оно работает?

### Безопасность

1. Какие виды уязвимостей знаешь?
1. Что такое `XSS` уязвимость? Как организовать защиту от неё?
1. Что такое `SQLi` уязвимость? Как организовать защиту от неё?
1. Чем HTTPS отличается от HTTP?

## Middle

### Общие вопросы

1. В чем разница между аутентификацией, авторизацией и идентификацией?
1. Расскажи о принципах SOLID.
1. Расскажи о принципах ООП.
1. Какие паттерны программирования знаешь? Приведи пару примеров.
1. Достаточно ли валидации в ORM при реализации проверки на уникальность, например, email при регистрации? Раскройте
1. Какие последствия возможны при отправке email прямо в контроллере? Как можно решить эти проблемы?
1. Как бы вы реализовали смену email на сайте, так чтобы соблюсти баланс между сложностью и безопасностью?
1. Можно ли доверять email, который мы получаем по oauth от соц сетей и мержить аккаунты автоматически? Приведите примеры
1. Как ограничить отправку email пользователю, который добавил письмо нашего проекта в спам? И почему это стоит делать (или не стоит)?
1. Предположим что вы реализуете редакцию журнала, где редактора могут в админке править статьи. Как предотвратить ситуацию, когда два редактора могут начать одновременно редактировать одну статью и перетирать изменения друг друга?
1. Каких принципов разработки нужно придерживаться, для обеспечения механизма zero downtime deployment. Как это достигается?
1. Что может произойти, если ваша `cron` задача, которая запускается раз в минуту, стала выполняться больше 1 минуты? Как это можно предотвратить?
1. Если вы пишите тесты, то как вы обходите проблему того, что код который вы тестируете, делает внешние вызовы? Доп условие, говорим о том, что на CI внешние вызовы запрещены (почему так правильно?)
1. Предположим что в вашей системе реализована смена емейла. При этом этот емейл хранится еще и во внешней системе, например эквайринге, который шлет пользователю свои письма (но пользователь им напрямую не пользуется). Как бы вы реализовали синхронизацию емейла с внешней системой?
1. Как вы узнаете об ошибках, которые происходят на продакшене? От пользователей или это автоматизировано?
1. Как обеспечивается изоляция тестов друг от друга если они ходят в базу и меняют ее? Если в вашем фреймворке этого нет, то как вы это делаете или сделали бы?

### Python

1. Как создать генератор в Python?
1. Чем тебе интересен Python? Почему выбрал эту технологию?
1. Расскажи про проекты, которыми занимался, и какие технологии использовал?
1. Как бы ты охарактеризовал Python? Какие преимущества или недостатки у него есть?
1. Как ты понимаешь ссылочную модель в Python?
1. Если мы создадим переменную `a`, в которой будет значение `1`, и создадим переменную `b = a`, то сколько объектов и сколько ссылок будет создано?
1. Для чего нужен счетчик ссылок в Python?
1. Какие типы данных изменяемые, а какие неизменяемые в Python? Почему это важно?
1. Расскажи про использование моков
1. Какие есть способы расширить модель пользователя в Django?
1. Что такое класс `BaseView` и для чего он используется?
1. Как бы ты описал модель проектирования Django? Какие конструкции использует Django?
1. Как реализовать систему избранного в интернет-магазине на Django?
1. Как устроена система авторизации в Django?
1. Как реализовать корзину для интернет-магазина в Django?

### Безопасность

1. Какие типы `XSS` уязвимости ты знаешь?
1. Какие типы `SQLi` уязвимости ты знаешь?
1. Знаком с OWASP? Какая цель у этого проекта и чем он полезен разработчикам?
1. Расскажи про OWASP Top 10. Какие самые популярные уязвимости в этом рейтинге?

### Задачи

1. Как написать скрипт для скачивания 1000 картинок? Какие подходы лучше (асинхронно, несколько потоков и т.д.)?
1. Как бы ты оптимизировал скрипт для скачивания изображений и сделал из него микросервис?
1. Как реализовать обработку изображений в таком микросервисе?
1. Как написать код для подсчета четных чисел в списке?
1. Как работать с запросами, которые внезапно стали медленнее, особенно с `JOIN`?
1. Как обработать исключения при работе с файлами в Python (отсутствие файла, другие ошибки)?
1. Как реализовать обращение к API с ограничением по времени и количеству потоков?
