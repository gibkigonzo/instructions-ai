---
name: hotfix
description: "Szybki hotfix dla krytycznego błędu produkcyjnego."
agent: main-dev
---

Pomóż mi przeprowadzić hotfix krytycznego błędu produkcyjnego.

1. Najpierw poproś o:
   - opis błędu,
   - wpływ na użytkowników,
   - logi/stack trace,
   - wersję, na której występuje problem.
2. Zaproponuj minimalną zmianę naprawiającą błąd, z naciskiem na:
   - brak regresji,
   - brak zmian w zachowaniu poza tym przypadkiem.
3. Zaproponuj:
   - test(y), które potwierdzą naprawę,
   - plan rollbacku w razie problemów.
4. Oznacz w odpowiedzi, które fragmenty są „quick fix”, a co jest rekomendowane do późniejszego, pełniejszego refactoringu.
