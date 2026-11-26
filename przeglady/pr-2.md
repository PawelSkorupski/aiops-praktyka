# PR #2: web: nowa stopka
**Werdykt: MERGE**

## 3 najważniejsze powody
1. Zmiana ogranicza się do jednej linii statycznego HTML (`app/web/html/index.html:64`) — brak sekretów, obrazów, workflow, akcji GitHub i zmian w `resources`.
2. Opis PR-a jasno mówi, co się zmienia (tekst stopki) i dlaczego (informacja o dniach pracy Kantyny).
3. Checki CI nie są czerwone: testy orders-api i payments przechodzą, build i wdrożenie zostały pominięte (skipping) — żaden check nie jest `fail`.
## Blokery
- brak
## Uwagi
- brak
## Checki
| check | stan |
|---|---|
| Build ${{ matrix.service }} | skipping |
| Wdrożenie do ${{ vars.K8S_NAMESPACE }} | skipping |
| Testy orders-api | pass |
| Testy payments | pass |
