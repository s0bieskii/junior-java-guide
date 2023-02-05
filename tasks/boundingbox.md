# Bound inboxes

## Zadanie

Zadanie podesłane przez znajomego. Niestety nie mam do niego rozwiązania.

```
# REST API

## Cel

Celem wyzwania jest sprawdzenie umiejętności stworzenia REST API z wykorzystaniem Spring Boot.

## Opis zadania

Wyobraźmy sobie, że mamy zdjęcie. Na zdjęciu są narysowane bounding boxy. Nasze API ma umożliwiać operowanie na tych bounding boxach. Bounding boxy to obiekty, każdy z nich ma swój unikatowy **id**, **nazwę** i 2 **punkty** (lewy górny, prawy dolny róg), z kolei każdy punkt posiada współrzędne **x** i **y**. Do przechowywania bounding boxów wykorzystaj jedną ze struktur dostępnych w Javie.

Aplikacja Umożliwia:

* Dodanie bounding boxa
* usunięcie bounding boxa
* edycję bounding boxa (punkty i nazwa)
* pobranie konkretnego bounding boxa po id
* pobranie wszystkich bounding boxów

**Dodatkowo przy dodawaniu i edycji bounding boxów należy zwrócić uwagę:**

* nie można dodać bounding boxa poza zdjęciem
* nie można dodać bounding boxa jeśli nie spełnia on minimalnej wielkości

Ponadto aplikacja spełnia poniższe wymagania:

* Aplikacja otrzymuje i zwraca dane w formacie JSON
* Wykorzystuje odpowiednie metody oraz kody odpowiedzi HTTP
* id jest generowane automatycznie przez aplikację, nie podajemy go ręcznie przy dodawaniu nowych bounding boxów.

Wielkość zdjęcia oraz minimalna wielkość bounding boxów należy wczytać z pliku konfiguracyjnego yaml.

przykładowy config:

workspace:
image:
width: 1920
height: 1080
boundingBox:
minWidth: 10
minHeight: 10

## Wynik

Wynikiem zrealizowanego zadania powinien być projekt Gradle wykorzystujący Java oraz Spring Boot, spełniający powyższe wymagania.

## przydatne linki

* https://start.spring.io/ (dodaj zależność spring web)
* https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/
```