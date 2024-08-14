
## Вопросы для аналитиков данных

<details>
<summary>Перечислите порядок написания операторов в запросе SQL</summary>

```sql
SELECT
 [DISTINCT | DISTINCTROW | ALL]
 select_expression,...
 FROM table_references
 [WHERE where_definition]
 [GROUP BY {unsigned_integer | column | formula}]
 [HAVING where_definition]
 [ORDER BY {unsigned_integer | column | formula} [ASC | DESC], ...]
```
</details>

<details>
<summary>Перечислите порядок выполнения операторов в запросе SQL</summary>

```sql
1. FROM
2. WHERE
3. GROUP BY
4. HAVING
5. SELECT
6. ORDER BY
```
</details>

<details>
<summary>Назовите, чем отличаются операторы HAVING и WHERE</summary>
<p>HAVING используется как WHERE, но в другой части SQL-выражения и, соответственно, на другой
стадии формирования запроса. HAVING применяется не для всего набора столбцов таблицы, а для набора созданного оператором GROUP BY и применяется всегда строго после него.</p>
</details>

<details>
<summary>Назовите ключевые метрики вовлеченности продуктового анализа</summary>
TODO
</details>

<details>
<summary>Назовите, чем отличается оператор extend() от оператора append()</summary>
TODO
</details>

<details>
<summary>Какая библиотека используется для чтения и обработки табличных данных</summary>
TODO
</details>

<details>
<summary>Какой график выбрать для наиболее детального отражения структуры продаж (по категориям)? А если требуется </summary>
TODO
</details>
рассмотреть эту структуру в динамике (с течением времени)?
<details>
<summary>Можно ли соединить таблицу саму на себя?</summary>
TODO
</details>

<details>
<summary>Какой оператор помогает вывести ограниченный список значений в результате запроса?</summary>

```sql
SELECT id
FROM answer
LIMIT 10;
```
</details>

<details>
<summary>Какой минимальный и максимальный результат получится при соединении таблиц друг с другом</summary>
TODO
</details>

<details>
<summary>Объясните, что означает «связь таблиц «один ко многим»»?</summary>
TODO
</details>

<details>
<summary>Каким способом можно избавиться от дублей в таблице? Какие еще способы вы знаете?</summary>

```sql
    SELECT DISTINCT title
    FROM report;
```
```sql
    SELECT id, title, COUNT(*)
    FROM report
    GROUP BY id, title
    HAVING COUNT(*) = 1;
```
</details>

<details>
<summary>Напишите запрос, который посчитает количество заказов каждого клиента, который проживает в городе N и сумма </summary>
TODO
</details>
заказов превышает M рублей
<details>
<summary>Напишите запрос, который посчитает суммарную выручку компании по дням недели</summary>
TODO
</details>

<details>
<summary>Напишите запрос, который выведет всех сотрудников, у которых зарплата больше, чем у их руководителей</summary>
TODO
</details>

<details>
<summary>Напишите скрипт, который позволит найти накопленным итогом сумму расходов и доходов по продаже определенного </summary>
TODO
</details>
продукта
<details>
<summary>Написать скрипт, который позволит найти всех клиентов компании, которые одновременно являются сотрудниками этой </summary>
TODO
</details>
компании
<details>
<summary>Представим, что у вас есть доступ к данным о перемещениях ваших клиентов. Сформулируйте гипотезы (критерии), </summary>
TODO
</details>
которые позволили бы вам однозначно определить, где сейчас находится ваш клиент – в спортивном зале или в магазине?
<details>
<summary>Вам доступны данные по продукту N: все клики на сайтах, все cookies посетителей, все метки рекламных ссылок и </summary>
TODO
</details>
все зарегистрированные пользователи вашего сайта. Расскажите, какие метрики вы бы начали собирать для извлечения из данных полезных инсайтов? С чего бы вы начали решать эту большую задачу?
<details>
<summary>Сколькими способами можно разложить пять книг на одной полке?</summary>
TODO
</details>

<details>
<summary>Какова вероятность выпадения «орла» и «решки» при одновременном подкидывании двух монет?</summary>
TODO
</details>

<details>
<summary>Если взять число, затем уменьшить его на N%, затем увеличить полученное число на N%, каким получится итоговое </summary>
TODO
</details>
число – большим или меньшим первоначального числа? Как изменится ваш ответ, если выполнить шаги увеличения и уменьшения в обратном порядке?
<details>
<summary>Знаете ли вы, что такое математическое ожидание и как его найти для ряда чисел?</summary>
TODO
</details>

<details>
<summary>Чем отличается медиана от среднего значения? В каком случае лучше применить среднее, а в каком – медиану?</summary>
TODO
</details>

<details>
<summary>Чем отличается множество от списка?</summary>
TODO
</details>

<details>
<summary>Как можно развернуть в обратном порядке все элементы списка? Какие еще методы выполнения этой задачи вам </summary>
TODO
</details>
известны?
<details>
<summary>Что будет, если в Python попытаться сложить число 5 и значение NULL?</summary>
TODO
</details>

<details>
<summary>В чем разница между операторами any() и all()?</summary>
TODO
</details>

<details>
<summary>Как удалить все пробелы в строке? Каким еще способом это можно сделать?</summary>
TODO
</details>

<details>
<summary></summary>
TODO
</details>
