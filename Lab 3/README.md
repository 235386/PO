# Laboratorium #3

Utrwalenie wiadomości dotyczących klas. Operatory, konstruktory kopiujące, wyjątki.

## Materiały pomocnicze

http://www.cplusplus.com/doc/tutorial/templates/ (sekcja Overloading operators)
http://www.cplusplus.com/doc/tutorial/classes2/ (sekcja Copy constructor)
http://www.cplusplus.com/doc/tutorial/exceptions/

## Etap 1 (3.0)

Zaimplementuj klasę Vector, opisującą wektor liczb zmiennoprzecinkowych. Rozmiar wektora powinien być parametrem konstruktora. W konstruktorze powinna być rezerwowana pamięć, wartości wektora powinny natomiast być inicjalizowane zerami. Zarezerwowana pamięć powinna być zwalniana w destruktorze. Przeładuj operator tablicowy [] klasy Vector, umożliwiając odwoływanie się do poszczególnych elementów wektora i przypisywanie im wartości.

## Etap 2 (4.0)

Przeładuj operatory +, -, * oraz /, umożliwiając dokonywanie arytmetycznych na parach wektorów. Utwórz konstruktor kopiujący. Uwaga: nowo utworzony obiekt nie może współdzielić pamięci z obiektem źródłowym! Zadbaj o poprawne przydzielanie pamięci dla nowego obiektu.

## Etap 3 (5.0)

Przeładuj operator przypisania. Pamiętaj, że operator musi zwolnić pamięć obiektu docelowego i zaalokować nowy blok pamięci. Zabezpiecz napisany kod przed niepoprawnym wykonaniem: w przypadku operacji arytmetycznych sprawdzaj kompatybilność rozmiarów obiektów, w przypadku operatora tablicowego to, czy nie podany został indeks z poza zakresu, natomiast w przypadku operatora przypisania to, czy nie występuje przypisanie obiektu do samego siebie. Zadbaj o zwracanie odpowiednich wyjątków.

## Etap 4 (5.5)

Zaimplementuj wariant, w którym rozmiar wektora nie jest znany podczas inicjalizacji. W tym celu wykorzystaj dwie struktury danych: tablice i listy. Możesz wykorzystać gotową implementację listy. Podczas implementacji nowych klas wykorzystaj dziedziczenie. Które z operacji są lepsze (i pod jakim względem) w którym z wariantów?
