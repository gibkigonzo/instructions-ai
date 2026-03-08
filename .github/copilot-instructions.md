# GitHub Copilot – instrukcje repo

To repozytorium używa:
- Astro 4+ z TypeScriptem do renderingu stron i komponentów.
- Vitest do testów jednostkowych i integracyjnych, Playwright do E2E. 
- ESLint (z `eslint-plugin-astro`) oraz Prettier do spójnego stylu. 
- Node.js/Edge API routes (w katalogach z endpointami) do logiki backendowej.

## Ogólne zasady

- Zawsze respektuj istniejące konfiguracje: `astro.config.*`, `vite.config.*`, `vitest.config.*`, `eslint.config.*` lub `.eslintrc.*`, `.prettierrc.*`.
- Preferuj czysty, prosty kod zamiast sprytnych hacków; stawiamy na czytelność i testowalność.
- Każda nowa funkcjonalność powinna:
  - mieć sensowny podział na komponenty/partial-e,
  - posiadać testy (Vitest / Playwright – w zależności od charakteru),
  - nie psuć istniejących testów ani lintingu.
- Przy generowaniu kodu zwracaj uwagę na:
  - bezpieczeństwo (walidacja danych wejściowych, brak wycieków sekretów),
  - dostępność (a11y) i poprawną semantykę HTML,
  - performance (unikanie zbędnego JS na kliencie, wykorzystanie server-first podejścia Astro).
