# Subtask 1 - Krótki kurs podstaw SQL
----
https://www.kursysql.pl/sql-w-120-minut/

SELECT * FROM 

SELECT TOP

SELECT ProductID, Name, Color, Size 

FROM Production.Product

ORDER BY

# ﻿Subtask 2 - Konfiguracja środowiska i wgranie bazy danych
---
![image](https://user-images.githubusercontent.com/122563907/218429648-a5a4f02d-83c5-48b0-81b2-eafdda0aaa1c.png)

# ﻿Subtask 3 - Kilka zadań na rozgrzewkę
---
1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.

*SELECT * FROM actors ORDER BY surname;*

![image](https://user-images.githubusercontent.com/122563907/218438036-1e1674e9-1a20-41e1-a185-445dba92c5b8.png)

2. Wyświetl film, który powstał w 2019 roku.

*SELECT * FROM movies WHERE year_of_production= 2019;*

![image](https://user-images.githubusercontent.com/122563907/218438635-d9251302-e08c-4f2d-9dc1-0677e10722d9.png)

3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.

*SELECT * FROM movies WHERE year_of_production BETWEEN 1900 and 1999;*

![image](https://user-images.githubusercontent.com/122563907/218439236-9b1a59d4-e00e-4bb0-845c-32db31c734fe.png)


