# Live-coding task

## Zadanie

To zadnie robiłem jako live coding podczas rozmowy. Maksymalny czas na jego wykonanie to 35 minut.
Dostałem dwie klasy z komentarzami jako opisem mini zadań. Poniżej znajdziesz te klasy już z częściowo rozwiązanymi zadaniami, lecz nie wszystkie są rozwiązane dobrze lub najoptymalniej.
Zadania rozwiązałem na tyle dobrze, żeby dojść do kolejnego etapu rozmowy.

```java
public class L1 {
 
    /** Wytyczne do zadań:
     * - załóż, że dane wejściowe są poprawne, nie sprawdzaj warunków brzegowych,
     np. czy argumenty mają wartość null, lub czy tablice są puste;
     * - nie uruchamiaj kodu, nie pisz main'a ani unit testów
     * - nie wydzielaj osobnych metod ani stałych.
     */
 
 
    /**
     * Zwróć pierwszy element tablicy
     */
    public int firstElem(int[] array) {
        return array[0];
    }
 
    /**
     * Zwróć ostatni element tablicy
     */
    public int lastElem(int[] array) {
        return array[array.length-1];
    }
 
    /**
     * Zwróć wybrany element tablicy
     */
    public int elementAtIndex(int[] array, int index) {
        return array[index];
    }
 
    /**
     * Zwróć negację podanego parametru
     */
    public boolean not(boolean a) {
        return !a;
    }
 
    /**
     * Zwraca wynik operacji 'LUB' dla podanych wartości logicznych a i b
     */
    public boolean or(boolean a, boolean b) {
        return a || b;
    }
 
    /**
     * Dla podanej liczby  a, zwróć liczbę a zwiększoną o 21
     */
    public int addTwentyOne(int a) {
        return a + 21;
    }
 
    /**
     * Dla podanych liczb a i b, zwróć ich iloczyn
     */
    public int multiply(int a, int b) {
        return a * b;
    }
 
    /**
     * Metoda powinna zwrócić wartość 4 miliardy
     */
    public long returnFourBillion() {
        return Long.valueOf(4000000000L);
    }
 
    /**
     * Dla podanych napisów a i b, zwróć ich sklejoną wartość
     */
    public String concat(String a, String b) {
        return new StringBuilder().append(a).append(b).toString();
    }
 
    /**
     * Zwróć ostatni znak napisu
     */
    public char lastChar(String a) {
        return a.charAt(a.length());
    }
 
    /**
     * Zwróć wartość bezwzględną dla podanej liczby
     */
    public int abs(int a) {
        return Math.abs(a);
    }
 
    /**
     * Sprawdza, czy kwadrat podanej liczby jest większa od 0
     */
    public boolean squareIsGreaterThan0(int a) {
        return false;
    }
 
}
```

```java
public class L2 {
 
    /**
     * Zwróć sumę wszystkich elementów tablicy
     */
    public int sum(int[] array) {
        int sum = 0;
        for (int x = 0; x < array.length; x++) {
            sum += array[x];
        }
        return sum;
    }
 
    /**
     * Zwróć sumę co drugiego elementu tablicy począwszy od array[0],
     * czyli array[0] + array[2] + array[4] + ...
     */
    public int sumEverySecond(int[] array) {
        int sum = 0;
        for (int x = 0; x < array.length; x++) {
            if (x % 2 == 0) {
                sum += array[x];
            }
        }
        return sum;
    }
 
    /**
     * Zwróć sumę parzystych elementów tablicy
     * <p>
     * Przykład:
     * [5, 8, 9, 13, 12, 8] => 8 + 12 + 8 = 28
     */
    public int sumEvenValues(int[] array) {
        int sum = 0;
        for (int x = 0; x < array.length; x++) {
            if (array[x] % 2 == 0) {
                sum += array[x];
            }
        }
        return sum;
    }
 
    /**
     * Zwróć tablicę zawierającą parzyste elementy tablicy
     * <p>
     * Przykład:
     * [5, 8, 9, 13, 12, 8] => [8, 12, 8]
     */
    public int[] filterEvenValues(int[] array) {
        int[] even = new int[array.length];
        int addCounter = 0;
        for (int x = 0; x < array.length; x++) {
            if (array[x] % 2 == 0) {
                even[addCounter] = array[x];
                addCounter++;
            }
        }
        return even;
    }
 
    /**
     * Zwróć:
     * - true gdy wszystkie wartości parametru mają wartość true
     * - false, jeśli jakakolwiek wartość parametru ma wartość false
     */
    public boolean allTrue(boolean... value) {
        for (boolean x : value) {
            if (x == false) {
                return false;
            }
        }
        return true;
    }
 
    /**
     * Skleja wszystkie napisy z parametru
     */
    public String concat(String... a) {
        StringBuilder stringBuilder = new StringBuilder();
        for (String string : a) {
            stringBuilder.append(string);
        }
        return stringBuilder.toString();
    }
 
    /**
     * Sprawdza czy liczba 'number', zapisana w systemie dziesiętnym, zawiera cyfrę 'digit'.
     * <p>
     * Przykłady:
     * (number = 456, digit = 5) => true, bo 5 jest pośród 4,5,6
     * (number = 456, digit = 7) => false, bo 7 nie ma pośród 4,5,6
     *
     * @param number dowolna dodatnia liczba całkowita
     * @param digit  szukana cyfra, dozwolone wartości liczby digit to 0,1,2,3,4,5,6,7,8,9
     */
    public boolean containsDigit(int number, int digit) {
        String string = String.valueOf(number);
 
        return string.contains(String.valueOf(digit));
    }
 
    /**
     * Zwróć "stronę" tablicy,
     * tj. wycinek tablicy o maksymalnej wielkości pageSize
     * <p>
     * Przykład:
     * dla array = [5, 8, 9, 13, 3, 12, 8]
     * (pageSize = 2, pageNumberZeroBased = 0) => [5, 8]
     * (pageSize = 2, pageNumberZeroBased = 1) => [9, 13]
     * (pageSize = 3, pageNumberZeroBased = 0) => [5, 8, 9]
     * (pageSize = 3, pageNumberZeroBased = 1) => [13, 3, 12]
     */
    public int[] getPage(int[] array, int pageSize, int pageNumberZeroBased) {
        int totalPages = Math.abs(array.length / pageSize);
        int counter = 0;
        int[] toReturn = new int[array.length];
        for (int x = pageNumberZeroBased; x < pageSize+pageNumberZeroBased; x++) {
            if (x == array.length - 1) {
                return toReturn;
            } else {
                toReturn[counter] = array[x];
                counter++;
            }
        }
        return toReturn;
    }
 
    /**
     * Metoda określa możliwość udzielenia pożyczki w zależności od występujących warunków.
     * Pożyczka może być udzielona wtedy i tylko wtedy, gdy pożyczkobiorca ma pracę lub pracę posiada współmałżonek,
     * z którym pożyczkobiorca posiada wspólnotę majątkową.
     * <p>
     * Zadanie: poniższa implementacja jest formalnie prawidłowa, lecz niezbyt czytelna. Uprość jej implementację.
     *
     * @param hasJob            określa, czy kredytobiorca ma pracę
     * @param hasSpouse         określa, czy kredytobiorca jest w związku małżeńskim
     * @param spouseHasJob      określa, czy współmałżonek ma pracę
     * @param communityProperty określa, czy pomiędzy małżonkami występuje wspólnota majątkowa
     */
    public boolean loanApproved(boolean hasJob, boolean hasSpouse, boolean spouseHasJob,
                                boolean communityProperty) {
        if (!hasJob) {
            if (hasSpouse && spouseHasJob && communityProperty) {
                return true;
            } else {
                return false;
            }
        } else {
            return communityProperty;
        }
    }
}
```