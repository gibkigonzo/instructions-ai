# Security – instrukcje

Te zasady mają pierwszeństwo przed innymi, gdy wchodzą w konflikt.

- Zawsze przestrzegaj zasady najmniejszych uprawnień: funkcje i endpointy powinny robić tylko to, co muszą.
- Unikaj wstrzykiwania surowego HTML (np. `set:html`, `dangerouslySetInnerHTML`) bez bardzo wyraźnej potrzeby i silnego oczyszczania danych.
- Przy generowaniu linków i przekierowań dbaj o to, by nie były podatne na open redirect.
- Nie wstawiaj sekretów (kluczy, tokenów) do bundle frontendu ani do logów.
- Utrzymuj CSP i inne nagłówki bezpieczeństwa zgodne z konfiguracją projektu; nie obniżaj poziomu zabezpieczeń (np. `unsafe-inline`) bez explicite prośby użytkownika.
- W przypadku wątpliwości priorytet ma bezpieczeństwo nad wygodą – proponuj bezpieczniejsze rozwiązanie i wyjaśniaj kompromisy.
