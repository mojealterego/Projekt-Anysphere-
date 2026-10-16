# Security policy

Projekt znajduje się na etapie inicjalizacji. Nie ma potwierdzonego produkcyjnego wdrożenia.

## Zasady
- Least privilege, deny by default, tenant isolation.
- Nigdy nie umieszczać kluczy API, tokenów ani danych klientów w repozytorium.
- Uruchamianie nieufnego kodu wyłącznie w izolowanym środowisku.
- Każde narzędzie i integracja wymaga autoryzacji i limitów.
- Zmiany w IAM, sekrety, deploy i merge do chronionych gałęzi wymagają kontroli.

Zgłoszenia podatności: nie publikować szczegółów exploita w publicznym issue; użyć prywatnego kanału GitHub Security Advisories, jeśli zostanie włączony.
