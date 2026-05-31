# GEditor

Prosty edytor graficzny w jednym pliku HTML.

## Funkcje

- **Narzędzia**: Selector, Rect, Circle, Ellipse, Arrow, Text
- **Właściwości**: kolor obrysu (Stroke), grubość linii (Width)
- **Selekcja**: kliknięcie, przeciąganie, Ctrl+klik (wielokrotny wybór), Del/Backspace usuwanie
- **Uchwyty**: 4 rogi — przeciąganie zmienia rozmiar, również dla obróconych obiektów
- **Rotacja**: Shift+Ctrl+Scroll myszką
- **Flip**: przyciski Flip H / Flip V w panelu właściwości (tekst, obraz)
- **Przesuwanie warstw**: Home = na spód, End = na wierzch
- **Tekst**: dwuklik = edycja treści, pole FS = rozmiar czcionki, rozmiar zmieniany też uchwytem
- **Obrazy**: Import Image (lokalny plik), Ctrl+V (schowek — `getAsFile` + fallback `navigator.clipboard.read`), automatyczne skalowanie do 80% canvas
- **Cofanie**: Ctrl+Z (`saveState()` przed każdą modyfikacją, stos 50)
- **Zoom**: Ctrl+Scroll, suwak
- **Pan**: środkowy przycisk myszy lub Shift+lewy
- **Eksport**: PNG / WebP / JPG

## Struktura

- `/home/btc/Public/GEditor/index.html` — całość (HTML + CSS + JS)

## Użycie

Otworzyć w przeglądarce.
