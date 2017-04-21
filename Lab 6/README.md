# Laboratorium #6

Interfejsy - utrwalenie materiału.

## Materiały pomocnicze

[Tworzenie nowych typów wyjątków](http://www.cplusplus.com/doc/tutorial/exceptions/) - sekcja Standard exceptions

## Etap 1 (3.0)

Stwórz interfejs Stack zawierający wirtualne metody void push(Item* obj), void pop() oraz Item* get(), odpowiadające za, kolejno: umieszczanie elementu na stosie, usunięcie elementu ze stosu oraz zwrócenie aktualnego elementu. Stwórz klasę Item zawierającą prywatne pole name typu string oraz jednoargumentowy konstruktor z argumentem tego samego typu. Stwórz klasę ArrayStack implementującą stos oparty o tablicę. Klasa ArrayStack powinna dziedziczyć po interfejsie Stack. Jej konstruktor powinien przyjmować argument typu int, opisujący maksymalną wielkość stosu.

## Etap 2 (4.0)

Zadbaj o zwracanie wyjątków w przypadku wystąpienia błędu. Konkretnie, zaimplementuj wyjątki StackFullException (zwracany w sytuacji, w której użytkownik usiłuje dodać element na pełen stos), StackEmptyException (zwracany, gdy użytkownik usiłuje pobrać lub usunąć element pustego stosu) oraz WrongSizeException (zwracany, gdy podany rozmiar stosu < 0).

## Etap 3 (5.0)

Utwórz klasę DynamicArrayStack, rozmiar której będzie automatycznie zwiększany. Jej konstruktor powinien mieć jeden argument, starting_size, domyślnie przyjmujący wartość 0. Jeżeli użytkownik usiłuje dodać nowy element na pełen stos, jego aktualny rozmiar powinien zostać podwojony.
