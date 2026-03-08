---
applyTo: "src/pages/api/**,src/pages/*.ts,src/lib/server/**"
---

# Backend – instrukcje

Te instrukcje dotyczą:
- endpointów API (np. `src/pages/api/**`, `src/pages/*.ts` / routes z logiką serwerową),
- dowolnych funkcji serwerowych używanych w projektach Astro.

Zasady:
- Waliduj i sanityzuj wszystkie dane wejściowe przed użyciem (query params, body, headers, cookies).
- Nigdy nie ufaj danym pochodzącym z klienta – w tym id użytkowników, ceny, itp.
- Zwracaj sensowne kody HTTP i komunikaty błędów bez ujawniania szczegółów implementacyjnych.
- Dostęp do sekretów (tokeny, klucze API) zawsze przez zmienne środowiskowe, nigdy w kodzie źródłowym.
- Jeżeli logujesz błędy, nie loguj danych wrażliwych (hasła, tokeny sesji, pełne dane kart, itp.).
