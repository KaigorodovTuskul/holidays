# Праздничные дни по производственному календарю с 1991 по 2026 гг.
Праздничные дни по производственному календарю с 1991 по 2026 гг. (в формате *.xlsx, *.csv, *.pickle, *.json, *.txt)<br>
Столбцы датафрейма:<br> day - день int,<br> month - месяц int,<br> year - год int,<br> date - дата в формате '%d.%m.%Y' datetime,<br> weekday - день недели int (порядок от 0 до 6, где 0 - понедельник, 6 - воскресенье)
Пример использования в python из формата *.csv:
```python
     day  month  year       date  weekday
0      1      1  1991 1991-01-01        1
1      2      1  1991 1991-01-02        2
2      7      1  1991 1991-01-07        0
3     25      2  1991 1991-02-25        0
4      8      3  1991 1991-03-08        4
```
## Examples
Пример использования в python из формата *.csv:
```python
import pandas as pd

df = pd.read_csv('holidays.csv')
#sep установлен по умолчанию ','. index_col также указывать нет необходимости.
```
Пример использования в python из формата *.pickle:
```python
import pandas as pd

df = pd.read_pickle('holidays.pickle')
```
Пример использования в python из формата *.txt:
```python
import pandas as pd

df = pd.read_csv('holidays.txt', sep='\t')
```
Пример использования в python из формата *.json:
```python
import pandas as pd

df = pd.read_json('holidays.json')
```
### Зачем?
Чтобы было.

## Источники
c 1993 по 2024 гг.: https://www.consultant.ru/law/ref/calendar/proizvodstvennye/ <br>
с 1991 по 1993 и с 2024 по 2006 гг.: сторонние ресурсы
