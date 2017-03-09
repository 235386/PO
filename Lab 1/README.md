# Laboratorium #1

Wyświetlanie macierzy losowych liczb. Powtórzenie wiadomości z poprzedniego semestru: tablice, wskaźniki, pętle, funkcje, struktury danych, operacje wejścia/wyjścia, operacje na plikach...

## Materiały pomocnicze

[Wprowadzenie do Visual Studio](https://msdn.microsoft.com/pl-pl/library/jj620919.aspx)  

[Generowanie liczb (pseudo)losowych](http://www.cplusplus.com/reference/cstdlib/rand/)  

[Określanie precyzji wyświetlanych liczb zmiennoprzecinkowych](http://www.cplusplus.com/reference/cstdio/printf/)  

[Struktury danych](http://www.cplusplus.com/doc/tutorial/structures/)  

[Zapisywanie do pliku](http://www.cplusplus.com/reference/cstdio/fprintf/)  

## Etap 1 (3.0)

Pobierz od użytkownika wymiary macierzy (wysokość i szerokość). Utwórz dynamiczną, dwuwymiarową tablicę liczb zmiennoprzecinkowych i wypełnij ją losowymi liczbami z zakresu [-1; 1]. Napisz funkcję jako parametry przyjmującą macierz oraz jej wymiary, wypisującą wartości macierzy na ekran. Wykorzystaj podaną funkcję do wyświetlenia macierzy. Pamiętaj o zwolnieniu pamięci przed zakończeniem programu!

## Etap 2 (4.0)

Podczas wyświetlania macierzy ogranicz liczbę miejsc po przecinku do 3. Następnie zamiast liczb zmiennoprzecinkowych wykorzystaj liczby zespolone. W tym celu utwórz specjalną strukturę danych, zawierającą pola odpowiadające części rzeczywistej i urojonej.

## Etap 3 (5.0)

Napisz funkcję zapisującą macierz do pliku tekstowego. Nazwa pliku powinna być jednym z parametrów funkcji. Następnie zmodyfikuj kod programu w taki sposób, aby w zależności od decyzji użytkownika zawartość macierzy była wyświetlana na ekran lub zapisywana do pliku. Nazwa pliku powinna być pobierana od użytkownika.
