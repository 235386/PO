# Laboratorium #4

Kompozycja, wstęp do dziedziczenia.

## Materiały pomocnicze

http://www.cplusplus.com/doc/tutorial/inheritance/ (sekcja Inheritance between classes)

## Etap 1 (3.0)

Zaimplementuj klasę Point, reprezentującą punkt w dwuwymiarowej przestrzeni. Jego współrzędne powinny być parametrem konstruktora. W definicji konstruktora wykorzystaj słowo kluczowe this. Utwórz metody zwracające wartość poszczególnych współrzędnych. Utwórz klasę Rectangle, która w konstruktorze przyjmuje punkty reprezentujące lewy górny i prawy dolny wierzchołek prostokąta. Napisz metodę getArea, zwracającą pole danego prostokąta. Przetestuj poprawne działanie napisanych klas.

## Etap 2 (4.0)

Napisz klasę Square, dziedziczącą po klasie Rectangle. Klasa Square, poza konstruktorem analogicznym do tego z klasy Rectangle, powinna zawierać dodatkowy konstruktor dwuargumentowy. Jego pierwszym argumentem powinien być lewy górny wierzchołek kwadratu, zaś drugim jego szerokość. Przetestuj działanie napisanej klasy.

## Etap 3 (5.0)

Napisz metodę collide dla klasy Rectangle, przyjmującą jako argument inny obiekt danej klasy. Metoda ta powinna sprawdzać, czy dwa prostokąty się nie przecinają, lub czy jeden nie zawiera się wewnątrz drugiego. Przetestuj poprawne działanie metody, w tym dla obiektów klasy Square.

## Etap 4 (5.5)

Zaimplementuj klasę przechowującą kolekcję obiektów typu Rectangle. Napisz metodę getCollisions, zwracającą kolekcję par wzajemnie przecinających się obiektów. Zadbaj o to, aby ta metoda miała mniejszą złożoność obliczeniową niż O(n^2). Wskazówka: można to rozwiązać dzieląc przestrzeń siatką na mniejsze obszary. Możesz założyć, że wszystkie prostokąty będą leżeć wewnątrz [0; 1] x [0; 1].
