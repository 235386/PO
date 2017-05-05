# Laboratorium #8

Celem tego laboratorium będzie zaimplementowanie prostej gry komputerowej. Postać gracza będzie przemieszczać się po dwuwymiarowej planszy zbierając przedmioty i walcząc z przeciwnikami. Celem gry będzie pokonanie wszystkich przeciwników.

## Etap 1 (3.0)

W pierwszym etapie zaimplementujemy klasy składowe, reprezentujące obiekty w świecie gry. Będą to, kolejno: Player (klasa reprezentująca postać gracza, przechowująca jego aktualne punkty życia, kolekcję posiadanych przedmiotów oraz pozycję na mapie), Item (reprezentująca przedmioty znajdujące się na mapie lub w ekwipunku gracza, zawierająca informację o sile danego przedmiotu), Enemy (reprezentująca przeciwników, zawierająca informację o ich sile i pozycji) oraz Potion (reprezentująca znajdujące się na mapie przedmioty, zwiększające życie gracza).

Do zaimplementowania tych klas potrzebna będzie struktura Position, przechowująca dwuwymiarowe koordynaty na planszy. Konieczne będzie ponadto zaimplementowanie dwóch interfejsów: Object, po którym dziedziczyć będą wszystkie klasy, zawierający koordynaty na planszy danego obiektu (zmienna typu Position oraz odpowiednia metoda do pobrania jej wartości), oraz Interactive, zawierający wirtualną metodę interact(Player player), po którym dziedziczyć będą klasy Item, Enemy oraz Potion.

Klasa Item powinna zawierać zmienną strength, reprezentująca siłę danego przedmiotu. Jej implementacja metody interact powinna natomiast przenosić dany przedmiot do ekwipunku gracza i usuwać jego pozycję na mapie.

Klasa Enemy także powinna zawierać zmienną strength, reprezentującą siłę danego przeciwnika. Jej metoda interact powinna porównywać siłę przeciwnika z siłą gracza. Siła przeciwnika powinna być porównana z siłą gracza, a następnie w oparciu o wynik tego porównania powinien: zostać zabity przeciwnik, zostać zabity gracz, lub zostać obniżone punkty życia gracza (zaproponuj mechanizm obniżania punktów życia gracza).

Klasa Potion powinna zawierać zmienną vitality, reprezentującą liczbę punktów życia zwróconą przez dany Potion. Jej metoda interact powinna przywracać graczowi daną liczbę punktów życia i usuwać pozycję dany obiektu na mapie.

Klasa Player powinna zawierać aktualną liczbę punktów życia, kolekcję przedmiotów (dynamiczna tablica lub vector) oraz metodę zwracającą siłę gracza (suma wszystkich przedmiotów).

## Etap 2 (4.0)

W drugim etapie zaimplementujemy klasę Board, przechowującą informację o aktualnym stanie planszy. Powinna ona zawierać kolekcję obiektów typu Interactive (dwuwymiarowa tablica lub vector) oraz obiekt typu Player. Zaimplementuj metodę umożliwiającą wczytanie planszy z pliku tekstowego, zapisanie do pliku tekstowego, oraz wygenerowanie losowej planszy w oparciu o podane parametry (wymiary planszy, liczba obiektów poszczególnych typów, maksymalne wartości siły/żywotności obiektów typu Interactive).

## Etap 3 (5.0)

Wykorzystując klasy zaimplementowane w poprzednich etapach zaimplementuj logikę gry oraz interfejs użytkownika. Mapa powinna być wyświetlana w terminalu. Ruchy powinny być przechwytywane od gracza, w oparciu o nie przemieszczany powinien być obiekt klasy Player. W momencie wejścia na obiekt typu Interactive powinna być wywoływana stosowna metoda. Gra powinna się kończyć w momencie utraty wszystkich punktów życia przez gracza (przegrana) lub pokonania wszystkich przeciwników (wygrana).

## Etap 4 (5.5)

Zaimplementuj interfejs graficzny dla napisanej gry. Zaproponuj mechanizm przemieszczania się przeciwników (lepszy niż losowe przemieszczanie), uniemożliw kolizje.
