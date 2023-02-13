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

4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$

*SELECT title, price FROM movies WHERE price < 7;*

![image](https://user-images.githubusercontent.com/122563907/218440762-25106861-4826-402d-ac4f-c0e9cad05ad6.png)

5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.

*SELECT * FROM actors WHERE actor_id>= 4 and actor_id<= 7;*

![image](https://user-images.githubusercontent.com/122563907/218441232-479b8549-a482-4832-945b-9968de2b34c5.png)

6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.

*SELECT * FROM customers WHERE mod(customer_id,2) = 0;*

![image](https://user-images.githubusercontent.com/122563907/218441608-15a4a77a-93b5-4f78-91bb-fe2d58c27c6f.png)

7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.

*SELECT * FROM customers WHERE customer_id IN (1,3,5);*

![image](https://user-images.githubusercontent.com/122563907/218442194-4886b9eb-aba9-4acc-bcf3-6a402ec71754.png)

8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.

*SELECT * FROM actors WHERE name Like 'An%';*

![image](https://user-images.githubusercontent.com/122563907/218442476-590537a5-c439-475f-81d4-6853933fe941.png)

9. Wyświetl dane klienta, który nie ma podanego adresu email.

*SELECT * FROM customers WHERE email IS null;*

![image](https://user-images.githubusercontent.com/122563907/218442920-b3e9ab93-0150-4bf0-b8ff-19c8d203cf23.png)

10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.

*SELECT * FROM movies WHERE price > 9 AND movie_id BETWEEN 2 and 8;*

![image](https://user-images.githubusercontent.com/122563907/218443592-1d7a07bc-9010-44fd-91d0-34ce8f4e06ce.png)



