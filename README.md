# GEditor

GEditor to prosty, działający w przeglądarce edytor grafiki oparty na elemencie HTML `<canvas>`. Cała aplikacja znajduje się w jednym pliku — `index.html` — i nie wymaga instalowania zależności ani uruchamiania backendu.

## Funkcje

- rysowanie prostokątów, kół, elips, łuków i strzałek;
- dodawanie tekstu;
- import lokalnych obrazów oraz wklejanie obrazów ze schowka (`Ctrl+V`);
- wybór koloru obrysu i grubości linii;
- opcjonalne wypełnienie figur geometrycznych;
- zaznaczanie pojedynczych lub wielu obiektów (`Ctrl` + kliknięcie);
- przesuwanie, zmiana rozmiaru, obracanie i odbijanie obiektów;
- edycja położenia i rozmiaru zaznaczonego obiektu;
- edycja tekstu oraz parametrów łuku, w tym kątów i grotów;
- cofanie zmian (`Ctrl+Z`, do 50 stanów);
- zmiana kolejności warstw (`Home` — na spód, `End` — na wierzch);
- zoom od 10% do 500% oraz przesuwanie widoku;
- eksport do PNG, WebP lub JPG.

## Uruchomienie

Sklonuj repozytorium lub pobierz pliki, a następnie otwórz `index.html` w nowoczesnej przeglądarce:

```bash
git clone https://github.com/n6210/geditor.git
cd geditor
```

Można też uruchomić prosty lokalny serwer HTTP:

```bash
python3 -m http.server 8000
```

Po uruchomieniu serwera otwórz [http://localhost:8000](http://localhost:8000).

## Skróty i obsługa myszy

| Działanie | Obsługa |
| --- | --- |
| Cofnięcie zmiany | `Ctrl+Z` |
| Usunięcie obiektu | `Delete` lub `Backspace` |
| Zaznaczenie wielu obiektów | `Ctrl` + kliknięcie |
| Obrót zaznaczenia | `Ctrl` + scroll; `Shift` + `Ctrl` zmienia obrót o 5° |
| Zoom | suwak zoomu lub `Ctrl` + scroll bez zaznaczenia |
| Przesuwanie widoku | środkowy przycisk myszy albo `Shift` + lewy przycisk |
| Zmiana kolejności warstw | `Home` / `End` |
| Szybka zmiana wartości liczbowej | scroll nad polem; `Shift` zwiększa krok |

## Struktura projektu

```text
geditor/
├── index.html   # HTML, style i logika aplikacji
└── README.md    # dokumentacja
```

Projekt nie zapisuje sesji automatycznie. Eksport obrazu służy do zapisania gotowego rezultatu.
