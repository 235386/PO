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
