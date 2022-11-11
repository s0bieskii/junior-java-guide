# Roadmap for Junior Java Developer

## Contents
- [Start](#słowo-na-start)
- [Moja droga nauki](mystory.md)
- [Roadmap](#roadmapa)
- [Polecane materiały](#polecane-materiay)
  - [Core](#core)
  - [Maven & Gradle](#maven--gradle)
  - [Internet & protokół HTTP](#internet--http)
  - [SQL/NoSQL Databases](#sql--bazydanych)
  - [API & Rest API](#api--rest-api)
  - [GIT & kontrola wersji](#git--kontrola-wersji)
  - [Spring/Springboot](#spring)
  - [ORM](#orm)
  - [Testy](#testy)
  - [Clean Code & paradygmaty](#cleancode--paradydmaty)
  - [Wzorce projektowe](#wzorce-projektowe)
  - [Logowanie w aplikacji](#logowanie-w-aplikacji)
  - [Docker](#docker)
  - [Linux](#linux)
  - [Mikroserwisy](#mikroserwisy)
  - [Message Broker](#message-broker)
    
## Słowo na start
Niniejsza ściąga jest spisem moich porad i obserwacji z drogi
przebranżowienia na Junior Java Developera. Ściąga ta nie jest jedną jedyną w 100%
słuszną drogą nauki, a jedynie subiektywnymi sugestiami. </br>
Znajdziesz tutaj porady, polecane źródła do nauki, przydatne programy, roadmape oraz inne
materiały.

## Roadmapa

0. [Angielski](#angielski)
1. [Core](#core)
    - JVM
    - Podstawowa składnia
    - Typy danych, operatory i wyrażenia
    - Klasy
    - Instrukcje warunkowe
    - Operatory
    - Pętle
    - Tablice i kolekcje
    - Przetwarzanie danych
    - Praca na plikach
    - Streamy
    - Algorytmy
    - Polimorfizm, interfejsy i klasy wewnętrzne
    - Programowanie obiektowe
    - Typy generyczne
    - Programowanie współbieżne [podstawy]
    - Debugowanie
    - Garbage collector
    - JavaFX [nie obowiązkowo]
2. [Maven & Gradle](#maven--gradle)
3. [Internet & protokół HTTP](#internet--http)
4. [SQL/NoSQL Databases](#sql--bazydanych)
    - MySQL
    - Postgres
    - H2Database
    - NoSQL [podstawy]
5. [API & Rest API](#api--rest-api)
6. [GIT & kontrola wersji](#git--kontrola-wersji)
7. [Spring/SpringBoot](#spring)
    - Validation
    - Spring Web
    - Security
    - Spring Data
8. [ORM](#orm)
   - Spring Data JPA
   - Hibernate 
9. [Testy](#testy)
    - Junit
    - Mockito
    - Test containers [nie obowiązkowo]
10. [Clean Code & paradygmaty](#cleancode--paradydmaty)
    - KISS
    - SOLID
    - DRY
11. [Wzorce projektowe](#wzorce-projektowe)
    - builder
    - adapter
    - strategia
12. [Logowanie w aplikacji](#logowanie-w-aplikacji)
13. [Docker](#docker) [podstawy]
14. [Linux](#linux) [podstawy]
15. [Mikroserwisy](#mikroserwisy) [nie obowiązkowo]
16. [Message Broker](#message-broker) (RabbitMQ/Kafka) [nie obowiązkowo]

Nice to have:
1. [HTML & CSS](#html--css) 
2. Ogólna wiedza o komputerach 
3. Good research skills


Jest to roadmapa sugerowana przeze mnie, możesz poszperać w internecie za innymi roadmapami które bardziej będą Ci odpowiadać np:
- [https://roadmap.sh/](https://roadmap.sh/java)
- [https://clockworkjava.pl/](https://clockworkjava.pl/2020/09/pragmatyczny-plan-nauki-dla-ekosystemu-java/)
- [https://www.programujodpodstaw.pl/](https://www.programujodpodstaw.pl/roadmapa-programisty/) [płatne]
- [https://www.javappa.com/](https://www.javappa.com/)

## Polecane materiały
### Legenda
Mimo że staram się wybierać tylko dobre źródła, to znajdziesz tutaj źródła bardziej zalecane oraz mniej zalecane. 
Przy każdym z nich znajdziesz symbol, który odpowiadający ocenie danego źródła. Na ocenę wpływa jakość materiałów, ilość praktycznych zadań,
format materiałów.

| Oznaczenie    | Znaczenie                   |
| ------------- |-----------------------------| 
| :heart:       | Najbardziej zalecane źródło |
| :green_heart: | Średnio zalecane źródło     | 
| :blue_heart:  | Najmniej zalecane źródło    | 
> **Note**
> To, że źródło jest najmniej zalecane, nie znaczy, że jest złe! 

### Angielski 
Większość internetu jest w języku angielskim w tym potencjalne rozwiązania Twoich przyszłych problemów programistycznych, 
jak i dokumentacja techniczna, której prędzej czy później zaczniesz używać. <br/> Także podstawowa znajomość angielskiego będzie
niemalże niezbędna, a im lepiej władasz tym językiem, tym więcej drzwi się przed Tobą otworzy. Przez cały czas nauki 
Javy trzeba szlifować swój język poprzez czytanie artykułów (jeśli nie wszystko rozumiesz to wspomagać się tłumaczem), oglądanie 
filmów na YouTube w języku angielskim, słuchanie podcastów oraz naukę angielskiego.
- Polecam zainstalować plugin do przegląradki umożliwiający szybkie tłumaczenie tekstu na stronie internetowej
- Zamiast znanego Google Translate polecam mniej znany, ale naturalniej tłumaczący [DeepL](https://www.deepl.com/translator)
- :heart: Jeśli chcesz pod szlifować wymowę możesz śmiało wpadać na discord [English](https://discord.gg/english) gdzie spotykają się osoby z całego świata by razem rozwijać swój angielski
- Dobrym startem są również aplikacje mobilne takie jak Duolingo
- Jeśli chcesz przetłumaczyć formalne dokumenty (np. CV), w których nie ma miejsca na wpadki to warto pamiętać o istnieniu takich stron jak [Turbo Tłumaczenia](https://turbotlumaczenia.pl/)

Im szybciej zaczniesz otaczać się językiem angielskim, tym lepiej dla przyszłego Ciebie;)

### Core
- **Darmowe**
  - :heart: [Kurs Uniwersytetu Helsinki](https://www.mooc.fi/en/) - certyfikowany kurs z Uniwersytetu Helsinki. Jesteśmy prowadzeni przez kurs za rękę. Polecam ze względu na to, że mocno stawia na praktykę i robimy setki mniejszych lub większych zadań, których poprawność jest sprawdzana przez testy automatyczne.
  - :heart: [JetBrains Adacemy](https://hyperskill.org/tracks?category=2) - darmowy kurs od JestBrainsów (tylko przy rejestracji z reflinka np tego: [LINK](https://hyperskill.org/join/ad5ebfbb6))  
  - :blue_heart: [Udemy Java for Complete Begginers](https://www.udemy.com/course/java-tutorial/) - kurs video dla totalnie początkujących  na Udemy
  - :green_heart: [JavaStart](https://javastart.pl/baza-wiedzy/darmowy-kurs-java) - kurs Javy od podstaw w języku polskim
  - :blue_heart: [CodeAcademy](https://www.codecademy.com/catalog/language/java) - interaktywny kurs Javy, dotykający totalnych podstaw. Dzięki niemu można w łatwy sposób liznąć programowania, nawet jeśli masz umysł humanistyczny.
  - :green_heart: [PJWSTK](http://edu.pjwstk.edu.pl/wyklady/) - mimo że dość stare materiały to treściwe i udostępnione za darmo przez Polsko Japońską Akademię Technik Komputerowych. Znajdziesz tutaj nie tylko kurs Javy ale sporo innych wartościowych materiałów

- **Płatne**
  - :heart: [JavaStart](https://javastart.pl/kurs/java) - rozszerzony kurs od JavaStart 
  - :heart: [JetBrains Adacemy](https://hyperskill.org/tracks?category=2) - to samo co za darmo z reflinka wyżej, ale jeśli nie zdążyłeś w 3-miesięczny okres próbny, to możesz wykupić subskrypcję. Płacisz za dostęp do całej platformy i wszystkich kursó, dlatego jeśli szybko będziesz przerabiał materiał, to cena końcowa nie wyjdzie taka zła.

### HTML & CSS
- **Darmowe**
  - :heart: [Kurs HTML & CSS Pasja Informatyki](https://www.youtube.com/watch?v=k2IydkL3EOs&list=PLa_qAIEJBI00FKOQegmfv8D2SXd6v3ABh)
  - :heart: [Kurs Bootstrap Pasja Informatyki](https://www.youtube.com/watch?v=Lvxy5GaArvo)
  - :heart: [Kurs HTML & CSS Kanał o Wszystkim](https://www.youtube.com/watch?v=BBHQGNkOb5w&list=PL6aekdNhY7DCmEzy303ZDo31d9uSYDCTt)
  - :heart: [Bootstrap](https://getbootstrap.com/docs/5.2/getting-started/introduction/)

### Maven & Gradle
- **Darmowe**
  - :heart: [Apache Maven dla początkujących](https://www.youtube.com/watch?v=BBHQGNkOb5w&list=PL6aekdNhY7DCmEzy303ZDo31d9uSYDCTt)
  - :green_heart: [Maven i tajemnica pliku pom.xml](https://kobietydokodu.pl/7-maven-i-tajemnice-pliku-pom-xml/)
  - :green_heart: [Maven Baeldung](https://www.baeldung.com/maven)

### Internet & HTTP
- **Darmowe**
  - :heart: [Protokół HTTP - co warto wiedzieć?](https://www.youtube.com/watch?v=BBHQGNkOb5w&list=PL6aekdNhY7DCmEzy303ZDo31d9uSYDCTt) - może nie jest to tutorial, ale w pigułce podane są tematy, które MUSISZ wiedzieć! Temat HTTP będzie z Tobą przez całą karierę w IT ;)
  - :heart: [Niezbędnik Juniora protokół HTTP](https://kobietydokodu.pl/niezbednik-juniora-protokol-http/) - przystępnie opisany protokół HTTP na blogu Kobiety do Kodu
  - :blue_heart: [How the Internet Works in 5 Minutes](https://www.youtube.com/watch?v=BBHQGNkOb5w&list=PL6aekdNhY7DCmEzy303ZDo31d9uSYDCTt)
  - :green_heart: [Niezbędnik Juniora jak działa internet?](https://kobietydokodu.pl/niezbednik-juniora-jak-dziala-internet/)
  

### SQL & bazydanych
- **Darmowe**
  - :heart: [Learn SQL in 60 minutes](https://www.youtube.com/watch?v=p3qvj9hO_Bo)
  - :heart: [Kurs SQL - podstawy](https://www.youtube.com/watch?v=15q9R1lTqvI) - skoncentrowany, praktyczny poradnik o SQL, niestety brak jest zadań praktycznych, ale można poćwiczyć np. na Hackerrank lub na tzw. katas (linki poniżej)
  - :heart: [HackerRank SQL](https://www.hackerrank.com/domains/sql) - zadania z SQL w interaktywnym wydaniu. Podzielone na trudność, oraz tematy.
  - :green_heart: [SQL Kata](https://www.codewars.com/kata/search/sql?q=SQL&beta=false&order_by=sort_date%20desc) - są to zestaawy mini zadań praktycznych przygotowanych przez innych userów, podzielonych na trudność oraz tematy. Tak zwane **katas** można znaleźć 
  - :blue_heart: [Kurs SQL z Kanał o Wszystkim](https://www.youtube.com/watch?v=BcZmEaX8u3w&list=PL6aekdNhY7DA1wcv-k2MtZxasDeGlre57) - spoko kurs SQL, lecz nie porusza tylu zagadnień i tematów jak poprzednie kursy
  - :heart: [Spring Boot Java H2 Database](https://www.youtube.com/watch?v=8QBJMxyXIqc) - praktyczny tutorial, pokazujacy config H2 Database z naszym projektem
  - :green_heart: [Baza danych H2](https://www.baeldung.com/spring-boot-h2-database) - jest to lekki silnik bazy danych. który doskonale sprawdza się do mini projektów Springowych.

### API & REST API
- **Darmowe**
  - :heart: [Wszystko o REST API w Javie](https://www.youtube.com/watch?v=C1bC134GvQ8) - bardzo dobrze przedstawiona wiedza o Rest API od Mateusza Dąbrowskiego
  - :heart: [15 zasad przy budowie Rest API](https://www.sztukakodu.pl/15-zasad-przy-budowie-rest-api-za-ktore-deweloperzy-cie-pokochaja) - zwięźle i na temat przedstawiona konwencja tworzenia Rest API
  - :heart: [API tutorial](https://www.youtube.com/watch?v=P9b8-BrWdYs)
  - :green_heart: [Tworzenie Rest API w SpringBoot](https://www.youtube.com/watch?v=P9b8-BrWdYs) - w 60 minut Kamil Brzeziński przeprowadzi nas przez różne tematy i pokaże jak tworzy się Rest API w SpringBoot. Warto sobie obejrzeć nawet jak nie rozumiemy pewnych zagadnień, żeby mieć wyobrażenie, co robi API i do czego się je wykorzystuje.
  
### GIT & kontrola wersji
- **Darmowe**
  - :heart: [Kurs Gita w praktyce](https://www.youtube.com/watch?v=tvHVafvw16Y&list=PLj-pbEqbjo6AKsJ8oE2pvIqsb15mxdrxs) - kurs od Łysego z IT 
  - :heart: [Git i GitHub w 60 minut](https://www.youtube.com/watch?v=Ebe9D5zRkvM)
  - :heart: [Git & GitHub Tutorial for Beginners](https://www.youtube.com/watch?v=3fUbBnN_H2c)
  - :heart: [OhShitGit](https://ohshitgit.com/pl) - przy nauce Gita na pewno zdarzą Ci się fuck upy, które chciałbyś cofnąć, wtedy wchodzi on cały na biało: OhShietGit.com
  - :heart: [Git Katas](https://github.com/eficode-academy/git-katas) - w nauce najważniejsza jest praktyka, dlatego tutaj znajdziesz zestaw mini zadań do praktycznej nauki Gita!

### Spring

### ORM

### Testy

### CleanCode & pWEaradydmaty 

### Wzorce projektowe

### Logowanie w aplikacji 

### Docker
- *Darmowe*
  - :heart: [Kurs Dockera od Zaprogramuj Życie](https://www.youtube.com/watch?v=Bb9O_TFSZUU&list=PLj-pbEqbjo6ABYxLDCKqvo3e0flutpbCy)

### Linux 

### Mikroserwisy

### Message Broker

## Polecane źródła
- https://www.baeldung.com/
- https://refactoring.guru/
- https://www.youtube.com/c/Zaprogramuj%C5%BBycie
- https://javappa.com/
- https://nullpointerexception.pl/blog/
- http://edu.pjwstk.edu.pl/wyklady/
- https://kobietydokodu.pl/tag/java/

### Inne
- https://open.agh.edu.pl/kategorie/informatyka/?orderby=popularity
- https://www.pja.edu.pl/biblioteka/repozytoria
- https://ocw.mit.edu/search/?d=Electrical%20Engineering%20and%20Computer%20Science
- https://academicearth.org/computer-science/
- Kanały JUG na YouTube

## Polecane programy
- **[InteliJ IDEA](https://www.jetbrains.com/idea/)** - IDE idealne do Javy
- **[Postman](https://www.postman.com/)** - narzędzie do wysyłania requestów HTTP oraz testowania API
- **[Ditto Clipboard](https://apps.microsoft.com/store/detail/ditto-clipboard/9NBLGGH3ZBJQ?hl=pl-pl&gl=pl)** - pozwala przeglądać historię skopiowanych treści oraz zarządzać nimi.
- **[ConEmu](https://conemu.github.io/)** - wygodna nakładka na terminal, pozwalająca na wygodne korzystanie oraz personalizowanie konsoli
-  **[Grammarly](https://www.grammarly.com/)** - plugin automatycznie sprawdzający poprawność tekstu wraz z sugerowaniem poprawek.


