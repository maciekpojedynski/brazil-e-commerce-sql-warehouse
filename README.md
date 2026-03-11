# Brazil e-commerce data warehouse


## 📌 Opis projektu
Projekt polega na zaprojektowaniu, budowie oraz utrzymaniu magazynu danych (Data Warehouse) opartego na T‑SQL. Celem jest stworzenie stabilnego, skalowalnego i dobrze udokumentowanego środowiska, które w przyszłości zostanie rozszerzone o integrację z Google BigQuery w ramach kierunku rozwoju chmurowego.
Zakres projektu obejmuje:

projektowanie struktur magazynu danych,
tworzenie i utrzymanie tabel, widoków, procedur oraz procesów ETL,
optymalizację zapytań T‑SQL,
przygotowanie modelu pozwalającego na późniejszą migrację oraz replikację danych do BigQuery.



## 🔐 Zasady pracy i kontrola jakości (GitHub Rulesets)
W repozytorium obowiązuje rygorystyczny workflow zapewniający bezpieczeństwo kodu oraz jego spójność.
### ✔️ Zakaz bezpośredniego merge do test i main
Merge do gałęzi:

test
main

może odbyć się wyłącznie poprzez Pull Request, który musi zostać zatwierdzony przez właściciela projektu.
Bez wcześniejszej akceptacji PR przez opiekuna (reviewera głównego) merge jest niemożliwy.

## 🌿 Zasady tworzenia branchy
W projekcie obowiązuje jasna metodyka pracy oparta na feature branchach.
### ✔️ Każdy nowy branch tworzymy z dev

    git checkout dev
    git pull
    git checkout -b feat/nazwa-zmiany

### ✔️ Nazewnictwo branchy
Nowe funkcjonalności, np. tworzenie nowych tabel, widoków, procedur:

    feat/nazwa-zmiany

## 🧱 Standardy kodowania
Aby zachować spójność w całym repozytorium:
### ✔️ Nie używamy tabów
Tabulacja w projekcie to 2 spacje.
Stosujemy:

2 spacje = 1 poziom wcięcia,
zero tabulatorów w plikach .sql,
pliki powinny być formatowane jednolicie w każdym PR.

Możesz wymusić to w edytorze (VS Code, SSMS, DataGrip itp.).

## 🔁 Przepływ pracy (workflow)

Developer tworzy branch typu feat/... z dev.
Implementuje zmiany.
Tworzy Pull Request → dev.
Po zatwierdzeniu integracja trafia do test.
Po pozytywnych testach zmiany przechodzą z test → main (również po akceptacji).