# Rest API zarządzania produktami

## Zadanie

W tym [LINK](https://github.com/s0bieskii/product-variants/) znajdziesz rozwiązanie tego zadania, dzięki któremu dostałem ofertę pracy od firmy rekrutującej.
Problem, który napotkałem przy tym zadaniu to zrozumienie oznaczeń **M:N** po krótkiej inwestygacji znalazłem to: [LINK](https://stackoverflow.com/questions/3397349/meaning-of-nm-and-1n-in-database-design)
Kolejna rzeczy, która sprawiła mi trudność to logiczne zaprojektowanie relacji oraz Docker, podczas tego zadania miałem do czynienia z nim pierwszy raz dlatego musiałem ekspresowo się go nauczyć;)

```
Przygotować usługę backend (REST) - projekt zarządzania kartoteką produktową.

Kompletny produkt występuje w następującej hierarchii:

1. DEFINICJA MODELU - dane producena
(producent, typ, nazwa modelu, płeć...)
2. DEFINICJA WARIANTU - każdy model może mieć różne warianty (kolor producenta)
- np. czerwony, czarny, biała perła
3. DEFINICJA ROZMIARU - każdy wariant jest dostępny w różnych rozmiarach
- np. dla butów 41, 42 lub dla nart 170, 176
4. SŁOWNIK PŁCI
- dla DEFINICJI MODELU (M:N)
5. SŁOWNIK ROZMIARÓW
- dla DEFINICJI ROZMIARU (M:N)

TODO:
1. Przygotować strukturę bazy danych (silnik mysql)
2. Dorzucić kolumnę z aktualną ceną (z założeniem, że cena może być różna per wariant/rozmiar)
3. Przygotować płaski widok (sql view) zawierający kolumny (typ, producent, nazwa modelu, kolor, rozmiar, aktualna cena)
4. (opcjonalnie) Zaimplementować proces archiwizacji danych produktowych:
a. MODEL z wszystkimi WARIANTAMI i ROZMIARAMI
b. WARIANT ze wszystkimi ROZMIARAMI
c. ROZMIAR
5. Przygotować rest api
a. dla DEFINICJI CRUD + (opcjonalnie) przeniesienie do archiwum
b. dla SŁOWNIKÓW dodanie i usunięcie z założeniem, że nie można usunąć wykorzystywanej pozycji
6. Wykonać dokumentację techniczną (swagger)
7. (opcjonalnie) Konteneryzacja, przygotować:
a. Dockerfile dla usługi
b. Komendę do utworzenia obrazu
c. Docker-compose do uruchomienia całej usługi (db + usługa rest)

Rozwiązanie powinno zawierać:
1. Skrypty sql do utworzenia struktury bazy danych lub skonfigurować DDL w usłudze (spring.jpa.hibernate.ddl-auto)
2. Przykładowe dane wejściowe do DB w formie skryptu sql lub json
3. Skrypt sql do utworzenia widoku (TODO pkt 3)
4. Kod usługi backend
5. Informację jak poprawnie skonfigurować / odpalić projekt
```


