# TASK 1
Subtask 1
-------------------------
8

Subtask 3
--
Cześć, Mam na imię Monika. Wzięłam udział w tym Dare IT Challenge na ścieżce QA: Zostań Testerem Manualnym ponieważ chciałabym się sprawdzić. Zdobyć nowe doświadczenia. Poznać nie znane mi tajniki testów. Jak rónież chciałbym wzbogacić się o kolejny projekt 😎
🤑

Subtask 4
------
**Aplikacja  Scouts Panel jest to strona zwierajaca informacje na temat graczy. Odbytych meczach. Można też znaleźć informacje o sportowcach tj. wiek, pozycję jaką zajmują, ja również osiągniecia jakie uzyskali. W Aplikacji zawarte są też raporty z meczów.**

* Na stronie głównej Aplikacji można znaleźc link pomocniczny w którym można dodac graczy. Aktywność czyli ostatni dodani gracze, stwozone raporty. Przedstawione są również statystiki ilości graczy, meczów, raportów.**

* Aplikacji zmieniłabym ilość jezyków bo dwa to za mało 🙂

|​- ** BŁĘDY** 😨-​|

1.  Przy zakładaniu nowego gracza 
* można podać datę uodzenia z przyszłości albo podać bardzo starą datę, Gracz zostanie założony.
* brak kontroli przy uzupełnianiu wzrostu, można podać dowolną wartość oraz zapisują się dane z użyciem znaków +/- przed podaniem wartości albo pomiędzy liczbami.
* przy podawaniu wagi nie jest określona jednostka. 
* przeds nazwą imienia, nazwiska pozwala na użycie znaków specjalnych.
* przy uzupełnianiu wagi, można podać dowolną watość oraz przed podaniem wartości można używać znaki +/-.
* w dacię urodzenia można w podać rok urodzenia z pięciu cyfr.
* przy dodawaniu języka nie pojawia się lista wyboru albo nie uzupełnia się automatycznie przy wpisywaniu.
* przy dodawaniu linku Youtube można wpisywać dowolne wartośc i znaki specjalne.
* przy dodawaniu profilu na Facebook można wpisywać dowolne wartości i znaki specjalne.
* przy wadze i przy wzroście nie ma określonego ilości znaków albo jest bardzo duża, moża podać dowolną wartość.
* to samo jest przy pozostałych informacjach np. osiągnieciach, klub, główna pozycja, nie ma określonej ilości znaków. 
* przy edycji gracza i po zapisawaniu pojawia sie komunikat NIE UDAŁO SIĘ ZAKTUALIZOWAĆ GRACZA, nie pojawia sie informacja co zostało bŁędnie uzupełnione.

2. Przy ściganiu graczy Download CSV, ściągają się tylko z pierwszej strony gracze.
* raport graczy w kolumnach Mecze "[object Object]"  
* raport dla pojedynczego gracza w kolumnach Mecze i Raporty pojawiają sie błędne opisy " [object Object]"

3. Przy drukowaniu graczy, w podglądzie wydruk pojawiają sie graczy tylko z pierwszej strony.
4. Jeśli przy dodawaniu meczu zostało coś błędnie podane to nie pojawia się informacja jakie pola są błędne. Zostało podana błędna data meczu rok był z 6 znaków a przy zapisie nie pokazała się informacja, że te pole jest błędne.
5. W zakładce mecze jest coś takiego jak Rozpocznij mecz po rozpoczęciu i uzupełnieniu graczy. Po wysłanniu raportu nie widomo gdzie on się znalazł 😞
