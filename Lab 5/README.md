# Laboratorium #5

Klasy abstrakcyjne, wielokrotne dziedziczenie.

## Materiały pomocnicze

[Klasy abstrakcyjne](http://en.cppreference.com/w/cpp/language/abstract_class)

[Wielokrotne dziedziczenie](http://www.cplusplus.com/doc/tutorial/inheritance/)

## Etap 1 (3.0)

Stwórz interfejs Printable udostępniający publiczną, wirtualną metodę print(std::ostream& stream). Stwórz klasę User zawierającą pola id oraz name, przekazywane jako parametry konstruktora. Klasa User powinna dziedziczyć po interfejsie Printable i implementować odziedziczone metody wirtualne. Metoda print klasy User powinna wyświetlać komunikat w formacie "[#id] name".

## Etap 2 (4.0)

Stwórz interfejs Accessible, implementujący funkcjonalność związaną z przyznawaniem uprawnień. Powinien on zawierać metody setAccess(int access), getAccess() oraz checkAccessible(int access). Pierwsze dwie powinny, odpowiednio, ustawiać uprawnienia obiektu (zakodowane jako liczba całkowita) lub je zwracać. Metoda checkAccessible powinna natomiast sprawdzać, czy dany obiekt ma odpowiedni poziom uprawnień, to znaczy czy jego uprawnienia są większe lub równe niż te podane jako argument metody. Rozszerz klasę User tak, aby dziedziczyła zarówno z Printable jak i Accessible, zaimplementuj też wszystkie metody wirtualne.

## Etap 3 (5.0)

Zmodyfikuj kod z poprzednich etapów w taki sposób, aby do kodowania uprawnień używane były nie liczby całkowite, ale enum przyjmujący wartości ze zbioru { low, medium, high, full }. Zmodyfikuj implementację metody wirtualnej print klasy User w taki sposób, aby wyświetlany był także poziom uprawnień. Zaimplementuj klasę Admin dziedziczącą z klasy User, którego uprawnienia zawsze są maksymalne. Próba modyfikacji uprawnień powinna rzucić wyjątek.
