# google_maps

PL:
Projekt przetwarza dane zebrane poprzez system czujników podłączonych do mikrokontrolera na trasie pojazdu odbierającego i przewożącego odpady i na ich podstawie wyrysowuje markery odzwierciedlające przebytą drogę na Mapie Google (odpowiednie ikonki w miejscach  załadunku/wyładunku odpadów). Dodatkowo z wzorcowego pliku pobierany jest wykaz miejsc, które przewoźnik miał obsłużyć i w razie niewypełnienia obowiązku na mapie wyświetlany zostaje odpowiedni znacznik. Dodatkowo w dwóch polach tekstowych wyświetlane zostają informacje o wykonanej pracy (adresy pojemników obsłużonych i pominiętych). System posiada szereg zabezpieczeń sprawdzających poprawność danych odebranych z mikrokontrolera - między innymi określanie, czy odczytane położenie geograficzne leży w obrębie Polski.

Aby poprawnie uruchomić aplikację należy:
- po wciśnięciu pierwszego z przycisków załadować plik RFID_codes_0.csv.
- po wciśniciu drugiego przycisku załadować któryś z plików:
    - test_0.txt.
    - test_0_1.txt.
    - test_1.txt.	
    - test_2.txt.
    - test_3.txt.
    - test_4.txt.
  każdy z nich pokazuje odmienną sytuację, pierwszy ilustruje poprawnie przebytą trasę, następne natomiast mają za zadanie zademonstrować   reakcję systemu na błędne dane bądź niepoprawnie odbyty kurs.
  
  Wykorzystano
  - HTML/CSS - do odpowiedniej wizualizacji danych i stworzenia interfejsu użytkownika,
  - JavaScript - do wczytywania danych z pliku, wszelkich algorytmów sprawdzania i przedstawiania danych,
  - Google Maps (w wersji 3.x) - do obsługi mapy, rysowania znaczników, umieszczania okien informacyjnych.
  
  
  PROGRAM OBSŁUGUJĄCY SYSTEM CZUJNIKÓW PODŁąCZONYCH DO MIKROKONTROLERA ZNAJDUJE SIĘ W REPOZYTORIUM 'ARDUINO MONITORING'
  
