# DOKUMENTACJA
## CHARAKTERYSTYKA OPROGRAMOWANIA
Nazwa skrócona: Labour market dashboard  
Pełna nazwa: Labour market dashboard for selected countries

Dashboard prezentuje wybrane wskaźniki dotyczące rynku pracy za pomocą różnorodnych wizualizacji. Jego celem jest wsparcie użytkowników w analizie trendów na rynku pracy oraz podejmowaniu decyzji dotyczących migracji zarobkowej. Dashboard zapewnia także funkcje analityczne, które ułatwiają zrozumienie globalnych różnic w wynagrodzeniach i warunkach pracy.

## PRAWA AUTORSKIE
Autorzy: Maria Kalkowska, Patrycja Kukułka  

Warunki licencyjne: oprogramowanie udostępniane na licencji MIT

## SPECYFIKACJA WYMAGAŃ
| Identyfikator | Nazwa                      | Opis                                                                                    | Priorytet | Kategoria     |
|---------------|----------------------------|-----------------------------------------------------------------------------------------|-----------|---------------|
| W1            | Pobieranie danych z API    | Aplikacja powinna umożliwiać poprawne pobranie danych z API ze strony OECD              | 1         | Funkcjonalne    |
| W2            | Analiza danych             | Aplikacja powinna analizować dane dotyczące rynku pracy oraz prezentować je w formie graficznej (np. wykresy, mapy) | 1         | Funkcjonalne   |
| W3            | Wizualizacja mapowa        | Aplikacja powinna zawierać wizualizację danych o realnych minimalnych płacach  na mapie świata | 1         | Funkcjonalne    |
| W4            | Podział na sekcje          | Aplikacja powinna zawierać podział na sekcje ze względu na przedstawiane dane           | 2         | Funkcjonalne    |
| W5            | Filtrowanie danych         | Aplikacja powinna umożliwiać filtrowanie danych według kraju oraz roku                  | 1         | Funkcjonalne    |
| W6            | Skalowalność               | Sposób zaprojektowania aplikacji powinien w łatwy sposób umożliwić jej rozszerzenie     | 2         | Pozafunkcjonalne|
| W7            | Wydajność systemu          | Aplikacja powinna działać w sposób płynny przy przetwarzaniu dużych ilości danych       | 1         | Pozafunkcjonalne|

## ARCHITEKTURA OPROGRAMOWANIA
| Nazwa            | Przeznaczenie                                                         | Wersja |
|------------------|-----------------------------------------------------------------------|--------|
| python           | język programowania                                                   | 3.11.5 |
| requests         | zapytania http                                                        | 2.31.0 |
| pandas           | ustrukturyzowanie i analiza danych                                    | 2.0.3  |
| dash             | stworzenie aplikacji                                                  | 2.18.2 |
| plotly express   | wizualizacja danych                                                   | 0.4.1  |
| jupyter notebook | platforma obliczeniowa                                                | 6.5.4  |

## TESTY
| Identyfikator | Nazwa                        | Opis  testu                                                                                                       |
|---------------|------------------------------|-------------------------------------------------------------------------------------------------------------------|
| T1            | Pobieranie danych z API OECD | Weryfikacja poprawności pobierania danych z API ze strony OECD                                                    |
| T2            | Wizualizacje danych          | Weryfikacja prezentacji danych na wykresach                                                                       |
| T3            | Wizualizacja mapowa          | Weryfikacja działania interaktywnej wizualizacji mapowej wraz ze zmianą w czasie                                  |
| T4            | Podział na sekcje            | Weryfikacja poprawności podziału aplikacji na sekcje                                                              |
| T5            | Filtrowanie danych           | Weryfikacja poprawności filtrowania danych pod względem lat i krajów                                              |
| T6            | Skalowalność                 | Weryfikacja umożliwienia łatwej rozbudowy aplikacji o nowe dane                                                   |
| T7            | Wydajność systemu            | Weryfikacja tego jak aplikacja radzi sobie ze zbiorem danych                                                      |

## SPRAWOZDANIE Z PRZEPROWADZONYCH TESTÓW
| Identyfikator | Wynik testu                  | Uwagi                                                                                           |
|---------------|------------------------------|-------------------------------------------------------------------------------------------------|
| T1            | Zakończony pozytywnie        | Dane zostały pobrane poprawnie                                                                  |
| T2            | Zakończony pozytywnie        | Dane były poprawnie i czytelnie zwizualizowane na wykresach                                     |
| T3            | Zakończony pozytywnie        | Wizualizacja mapowa była poprawnie zwizualizowana, a zmiana czasu poprawnie działała            |
| T4            | Zakończony pozytywnie        | Aplikacja została poprawnie podzielona na sekcje ze względu na prezentowane dane                |
| T5            | Zakończony pozytywnie        | Zarówno filtry lat jak i krajów poprawnie filtrowały dane                                       |
| T6            | Zakończony pozytywnie        | Aplikacja umożliwia łatwą rozbudowę, pozwalając powiększyć ją o nowe dane                       |
| T7            | Zakończony pozytywnie        | Aplikacja działa płynnie bez zauważalnych opóźnień                                              |
