# sleapyTV Donate Component

Prosty komponent rozszerzenia Twitch wyświetlający klikalny baner do donacji.

## Pliki

- `config.html` - strona konfiguracji rozszerzenia.
- `video_component.html` - komponent wideo wyświetlający baner i otwierający stronę donacji.
- `donate_banner.jpg` - grafika tła banera.
- `sleapytv-donate.zip` - paczka rozszerzenia, jeśli korzystasz z gotowego archiwum.

## Własny link do donacji

Przed przesłaniem plików otwórz `video_component.html` i zastąp tekst `PLESE ADD YOUR DONATE LINK` własnym adresem do donacji. Występuje on w dwóch miejscach w tym pliku; zaktualizuj oba.

## Własny baner

Przygotuj własną grafikę i dodaj ją do paczki rozszerzenia w Twitch Developer Console pod dokładną nazwą `donate_banner.jpg`. Kod komponentu odwołuje się do tej nazwy, więc nie zmieniaj jej bez aktualizacji ścieżki w `video_component.html`.

## Konfiguracja w Twitch Developer Console

1. Otwórz Twitch Developer Console i wybierz swoje rozszerzenie.
2. Wgraj `config.html` jako stronę konfiguracji oraz `video_component.html` jako komponent wideo.
3. Dodaj do paczki `donate_banner.jpg` oraz pozostałe wymagane pliki rozszerzenia.
4. Zapisz zmiany i sprawdź komponent w podglądzie rozszerzenia.

Komponent korzysta z Twitch Extension Helper: `https://extension-files.twitch.tv/helper/v1/twitch-ext.min.js`.
