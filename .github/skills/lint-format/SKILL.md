---
name: lint-format
description: "Naprawa błędów lintingu i formatowania zgodnie z konfiguracją ESLint/Prettier w tym projekcie."
user-invocable: false
---

## Zasady

- Zawsze respektuj istniejące konfiguracje:
  - ESLint (w tym reguły `eslint-plugin-astro` dla plików `.astro`),
  - Prettier i inne narzędzia formatowania.
- Przy poprawkach:
  - skupiaj się na minimalnych zmianach potrzebnych do usunięcia błędów,
  - nie refaktoruj logiki, chyba że użytkownik o to wyraźnie poprosi.
- Nie wyłączaj reguł linta (np. `// eslint-disable`) bez mocnego uzasadnienia.

## Procedura

1. Zidentyfikuj błędy lintingu/formatowania opisane przez użytkownika lub przez narzędzia.
2. Zaproponuj poprawki tak, aby:
   - były zgodne z obowiązującymi regułami,
   - nie zmieniały znaczenia kodu.
3. Jeżeli reguły wydają się nadmiernie restrykcyjne, opisz to w komentarzu zamiast je samodzielnie wyłączać.
