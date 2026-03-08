---
name: code-review
description: "Prowadzenie pełnego code review zmian w repozytorium."
user-invokable: true
argument-hint: "[lista plików / opis PR / diff]"
---

## Cel

Pomóc wykonać rzetelne code review w tym projekcie.

## Kiedy używać

- Gdy użytkownik prosi o review PR-a lub zestawu zmian.
- Przy self-review przed utworzeniem PR.

## Procedura

1. Przeczytaj kontekst zmian (diff, opis, powiązane issue).
2. Sprawdź:
   - poprawność logiki (frontend i backend),
   - testy (czy istnieją, czy pokrywają istotne ścieżki),
   - zgodność ze stylem i strukturą projektu,
   - potencjalne problemy bezpieczeństwa i performance.
3. Skategoryzuj uwagi:
   - `must-fix` – krytyczne błędy,
   - `should-fix` – ważne, ale nieblokujące,
   - `nice-to-have` – sugestie ulepszeń.
4. Zaproponuj, gdzie warto dodać lub poprawić testy.

## Format odpowiedzi

- Sekcja „Podsumowanie” (1–2 akapity).
- Sekcja „Uwagi” z listą punktów (`must-fix` / `should-fix` / `nice-to-have`).
- Sekcja „Rekomendacja” (np. „Gotowe po poprawkach must-fix”).
