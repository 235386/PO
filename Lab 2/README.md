# Laboratorium #2

Klasy. Definiowanie klas, konstruktory, destruktory, metody. Prawa dostępu (public i private).

## Materiały pomocnicze

http://www.cplusplus.com/doc/tutorial/classes/ (do sekcji Overloading constructors, włącznie) oraz http://www.cplusplus.com/doc/tutorial/classes2/#destructor (jedynie sekcja Destructor)

## Kartkówka - przykładowe pytania

```c++
#include <iostream>

using namespace std;

class Rectangle {
    int width, height;
  public:
    Rectangle();
    Rectangle(int, int);
    int area() { return (width * height); }
};

Rectangle::Rectangle() { }

Rectangle::Rectangle(int a, int b) {
  width = a;
  height = b;
}

int main() {
  Rectangle rect_a();
  Rectangle rect_b(5, 6);
  
  cout << rect_a.area() << endl;
  cout << rect_b.area() << endl;
  cout << rect_b.width * rect_b.height << endl;
  
  return 0;
}
```

Co zostanie wypisane w poszczególnych liniach (w przypadku błędów - uzasadnienie co poszło nie tak)? Jak sprawić, żeby ostatnia linia zadziałała prawidłowo? Pytanie bonusowe (nie obejmuje materiały z kartkówki): dlaczego może nie być to dobry pomysł?

## Etap 1 (3.0)

Utwórz klasę Logger, zadaniem której będzie logowanie komunikatów do pliku tekstowego. Konstruktor tej klasy powinien być odpowiedzialny za otwieranie wyjściowego pliku, destruktor - za jego zamykanie. Nazwa pliku powinna być parametrem konstruktora. Napisz metodę append, dopisującą komunikat w nowej linii pliku tekstowego. Argument tej metody powinien mieć typ [string](http://www.cplusplus.com/reference/string/string/). Przetestuj działanie napisanej klasy logując kilka komunikatów.

## Etap 2 (4.0)

Utwórz klasę Message, zadaniem której będzie przechowywanie treści logowanej wiadomości. Jej konstruktor powinien mieć pojedynczy argument o nazwie body i typie string. Napisz metodę get, zwracającą treść komunikatu podanego w konstruktorze. Zmodyfikuj metodę append klasy Logger w taki sposób, aby zamiast argumentu typu string przyjmowała argument typu Message.

## Etap 3 (5.0)

Zmodyfikuj klasę Message. Konstruktor powinien przyjmować dodatkowy argument o typie string, zawierający typ logowanego komunikatu (error, warning lub notification). W konstruktorze powinien być ponadto zapisany czas utworzenia danego obiektu (w tym celu możesz wykorzystać bibliotekę [ctime](https://www.tutorialspoint.com/cplusplus/cpp_date_time.htm)). Zmodyfikuj metodę get, tak aby zwracała ona wiadomości w formacie [Typ logowanego komunikatu][Rok-Miesiąc-Dzień Godzina:Minuta:Sekunda] Treść komunikatu.
