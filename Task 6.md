# Subtask 1 - Krótki kurs podstaw SQL
----
11. Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd 🙈

Przed zmianą 

![image](https://user-images.githubusercontent.com/122563907/219456145-09e7c02e-2a43-4519-af9d-38cbcd0ee0d1.png)

Po zmianie

*UPDATE customers set surname = 'Miler' WHERE customer_id = 3;*

![image](https://user-images.githubusercontent.com/122563907/219457569-719bc540-5451-479b-a374-b2343009ddd3.png)


12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.

*SELECT customers.name, customers.email FROM customers INNER JOIN sale ON customers.customer_id=sale.customer_id WHERE sale.movie_id=4;*

![image](https://user-images.githubusercontent.com/122563907/219650223-461f3481-9a16-43e8-9969-dba6c1a427c4.png)

13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com

*UPDATE customers set email = 'pati@mail.com' WHERE name = 'Patrycja'*

![image](https://user-images.githubusercontent.com/122563907/219651208-6a96c1ec-609f-498d-a7af-b80d5bc98a81.png)

14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).

*SELECT customers.name, customers.surname, movies.title FROM customers inner JOIN sale ON customers.customer_id = sale.customer_id inner JOIN movies ON movies.movie_id = sale.movie_id;*

![image](https://user-images.githubusercontent.com/122563907/219651722-8b739d8c-99e2-4b4a-86f5-270e99d2b8ac.png)

15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag

*ALTER TABLE customers ADD pseudomyn VARCHAR(3); UPDATE customers SET pseudomyn= CONCAT(SUBSTRING(name,1, 2), SUBSTRING(surname, -1))*

![image](https://user-images.githubusercontent.com/122563907/219874511-fbaf0aba-e4a2-45a3-9e23-584da1f4c654.png)

16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.

*SELECT DISTINCT movies.title from sale, movies WHERE movies.movie_id = sale.movie_id;*

![image](https://user-images.githubusercontent.com/122563907/219652668-65c8abaa-c2db-4695-8ce4-3f4184afbc1e.png)

17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)

*SELECT name FROM customers UNION SELECT name FROM actors ORDER BY name ASC;*

![image](https://user-images.githubusercontent.com/122563907/219874608-5058d1c7-a2dd-4f74-aa04-e91fb3dc9cb8.png)

18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).

Przed zmianą

![image](https://user-images.githubusercontent.com/122563907/219874773-dc1423b5-c150-4b91-a820-a3c67d18d407.png)

Po zmianie 

UPDATE movies SET price = price + 2.5 WHERE year_of_production > 2000

![image](https://user-images.githubusercontent.com/122563907/219874800-74e09fdb-98bd-456b-9adb-122236d86096.png)

19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał

SELECT actors.actor_id, actors.name, actors.surname, movies.title FROM actors INNER JOIN cast ON actors.actor_id=cast.actor_id INNER JOIN movies ON cast.movie_id=movies.movie_id WHERE actors.actor_id = 4;

![image](https://user-images.githubusercontent.com/122563907/219875160-a31e95df-16ad-4647-9a2f-45edf8df1163.png)

20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa

![image](https://user-images.githubusercontent.com/122563907/219875250-5bb1a059-95d3-4dfb-bd5d-ef9539d5f66d.png)

# Subtask 2 - Test
----
http://getistqb.com/quiz-seledynowy/

![image](https://user-images.githubusercontent.com/122563907/219451097-e78eed59-26f0-4308-9b68-0ab9db427cb7.png)

# Subtask 3 - Tworzymy portfolio

