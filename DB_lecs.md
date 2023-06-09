# БАЗЫ ДАННЫХ

<kbd>  </kbd>

`СУБД` это инструмент

Базы данных нужны для:
* хранения
* обработки
* быстрого извлечения

Пример **`иерархической модели хранения данных`**
```mermaid
    graph TD;
        A[художники]-->B[российские];
        B-->BA[авторы];
        BA-->BAA[...];
        B-->BB[жанры];
        BB-->BBA[год написания];
        BBA-->BBAA[...];
        BB-->D[пейзаж];
        BB-->E[натюрморт];
        BB-->F[портрет];
        A-->C[зарубежные];
        C-->CA[авторы];
        CA-->CAA[...];
        C-->CB[жанры];
        CB-->CBA[год написания];
        CBA-->CBAA[...];
        CB-->G[пейзаж];
        CB-->H[натюрморт];
        CB-->I[портрет];
        
```

**`Реляционные`** (relation - связь) базы данных - это бд, в которых данные распределены по отдельным, связанным мужду собой, таблицам.

**`SQL`** - особый язык программирования, который позволяет формулировать то, что нужно сделать с данными в таблицах.

ПРИМЕРЫ - пока используем **псевдокод**
___

SELECT * FROM Общий список

SELECT - "выбери"

\* - означает, что мы хотим видкть все столбцы

FROM - "из" - указываем, откуда необходимо выбрать инфрмацию

Общий список - название таблицы из нашего примера
___
SELECT ФИО, Тел, Комментарий

FROM Общий список
___
SELECT ФИО, Тел, Комментарий

FROM Общий список

WHERE статус = "холост"
___

![Извлечение данных из таблиц](extraction_data.png)

* INNER JOIN
    
        INNER JOIN Люди, Телефоны
        ON id = Чей телефон

    ___
* LEFT JOIN

        LEFT JOIN Люди, Адреса_2
        ON id = Чей адрес

    ___
* RIGHT JOIN

        RIGHT JOIN Люди, Адреса_2
        ON id = Чей адрес

    ___
* FULL JOIN
___

Взаимотношения
* 1 к 1
* 1 ко многим
* многий ко многим
* многие к одному
___
### Пример связей в реляционной модели
![Пример реляционной модели](example_relation_structure.png)

```mermaid

```
