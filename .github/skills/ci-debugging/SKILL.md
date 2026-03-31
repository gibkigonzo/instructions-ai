---
name: ci-debugging
description: "Analiza i debugowanie problemów z CI/CD (build, testy, deploy)."
user-invocable: true
argument-hint: "[logi, opis joba, nazwa pipeline'u]"
---

## Procedura

1. Poproś użytkownika o:
   - fragment logów z błędem,
   - nazwę joba/pipeline'u,
   - krótki opis ostatnich zmian.
2. Przeanalizuj logi:
   - czy błąd wynika z testów (Vitest/Playwright),
   - czy problem dotyczy builda Astro/Vite,
   - czy to kwestia środowiska (Node version, zmienne środowiskowe, zależności).
3. Zaproponuj:
   - konkretne poprawki w konfiguracji (skrypty, configi),
   - ewentualne zmiany w kodzie, jeśli to on powoduje błąd,
   - tymczasowe obejścia tylko z jasnym zaznaczeniem, że to workaround.
4. Jeżeli coś wymaga decyzji człowieka (np. zmiana strategii testów), wyraźnie to zaznacz.
