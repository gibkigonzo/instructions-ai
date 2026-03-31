---
name: astro-testing
description: "Pisanie testów dla komponentów i logiki w projekcie Astro z użyciem Vitest."
user-invocable: true
argument-hint: "[komponent, endpoint lub funkcja do przetestowania]"
---

## Kontekst

To repozytorium używa Vitest do testów jednostkowych i integracyjnych w projektach Astro.

## Zasady

- Wykorzystuj konfigurację Vitest z projektu (aliasy, pluginy) zamiast definiować ją od zera.
- Dla logiki:
  - pisz testy jednostkowe sprawdzające zachowanie funkcji (wejście/wyjście, edge case'y),
  - unikaj testów, które powielają oczywisty kod.
- Dla komponentów UI:
  - renderuj komponent i testuj zachowanie (tekst, interakcje, zmiana stanu),
  - używaj helperów/testing library przyjętych w projekcie.
- Dla E2E:
  - jeżeli proszony jest „test end‑to‑end”, zaproponuj szkic scenariusza dla Playwright (nawet jeśli kod idzie do osobnego pliku).

## Procedura

1. Zidentyfikuj publiczny surface testowanego elementu (API funkcji, propsy, oczekiwane renderowanie).
2. Wypisz najważniejsze przypadki:
   - scenariusz bazowy,
   - kluczowe edge case'y (puste dane, błędna konfiguracja),
   - przypadki błędów.
3. Zaproponuj lokalizację pliku testowego zgodnie z istniejącym wzorcem (np. `src/**/__tests__/*` lub `*.test.ts`).
4. Wygeneruj testy, które:
   - są czytelne,
   - nie polegają nadmiernie na snapshotach,
   - można utrzymywać w czasie.
