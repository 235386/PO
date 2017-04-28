# Laboratorium #7

Klasy szablonowe, metody statyczne.

## Materiały pomocnicze

http://www.cplusplus.com/doc/tutorial/templates/, sekcja Class templates

https://www.tutorialspoint.com/cplusplus/cpp_static_members.htm

## Etap 1 (3.0)

Zaimplementuj klasę Matrix reprezentującą macierz liczb całkowitych. Wymiary macierzy powinny być parametrami konstruktora. Zadbaj o poprawne zwalnianie pamięci, możliwość pobrania elementu na danej pozycji oraz przypisania mu zadanej wartości. Dla klasy Matrix utwórz statyczną zmienną o nazwie count, wewnątrz której przechowywany będzie licznik aktualnie istniejących macierzy (czyli - powinien być on dekrementowany w momencie zniszczenia obiektu). Utwórz statyczną metodę getCount, zwracającą wartość licznika.

## Etap 2 (4.0)

Zmodyfikuj klasę Matrix w taki sposób, aby była ona klasą szablonową. Przetestuj poprawność działania klasy dla różnych typów danych. Utwórz statyczną metodę readFromFile(std::string name, Matrix& obj), odczytującą zawartość macierzy z pliku tekstowego.

## Etap 3 (5.0)

Utwórz metodę statyczną writeToFile, zapisującą macierz do pliku tekstowego. Dodaj argument w konstruktorze, wartością którego będą inicjalizowane poszczególne pola macierzy. Zapewnij odpowiednią obsługę błędów (niepoprawne wymiary macierzy, odwoływanie się do nieistniejącego elementu, odczyt z nieistniejącego pliku...). Zaimplementuj operator przypisania oraz metodę wypisującą macierz na podany strumień.
