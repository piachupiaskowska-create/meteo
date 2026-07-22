# Meteogram

Prosta aplikacja pogodowa: **meteogram na 7 dni** dla dowolnej miejscowości. Bez backendu, bez klucza API — dane pobierane na żywo z [Open-Meteo](https://open-meteo.com).

## Funkcje

- Wyszukiwanie miejscowości (z rozróżnieniem, gdy nazwa pasuje do kilku miejsc).
- Aktualna pogoda + prognoza godzinowa na 7 dni w panelach:
  - temperatura (z odczuwalną),
  - opady i szansa opadów,
  - szansa burzy (szacunkowa, na podstawie CAPE i kodu pogody),
  - zachmurzenie,
  - wiatr i porywy,
  - wilgotność i ciśnienie.
- Ulubione miejsca zapisywane lokalnie w przeglądarce (`localStorage`).
- Przycisk „Moja lokalizacja" (geolokalizacja przeglądarki).
- Zoptymalizowane pod telefon; można dodać do ekranu głównego jako aplikację.

## Uruchomienie

Aplikacja to jeden plik `index.html`. Wystarczy otworzyć go w przeglądarce (wymagany internet — dane pobierane są na żywo).

### GitHub Pages

1. Wrzuć repozytorium na GitHub.
2. Settings → Pages → Source: `Deploy from a branch`, gałąź `main`, katalog `/ (root)`.
3. Po chwili aplikacja będzie dostępna pod `https://<login>.github.io/<repo>/`.

## Prywatność i bezpieczeństwo

- Aplikacja łączy się **wyłącznie** z `open-meteo.com` (HTTPS).
- Nie pobiera ani nie uruchamia zewnętrznego kodu.
- Używa jedynie internetu i (opcjonalnie, po Twojej zgodzie) lokalizacji przeglądarki. Nie sięga po żadne inne dane.

## Dane

Prognoza i geokodowanie: [Open-Meteo](https://open-meteo.com) (licencja danych: CC BY 4.0). Szansa burzy jest szacunkiem wyliczanym z CAPE i kodu pogody, nie oficjalną prognozą probabilistyczną.

## Licencja

MIT — zobacz [LICENSE](LICENSE).
