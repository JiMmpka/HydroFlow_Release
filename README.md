# HydroFlow

Dodatek do programu Microsoft Excel dla Windows do obliczeń przepływu w
kanalizacji: obliczenie przepływu, automatyczny dobór wymiarów kanałów i
spadków, dodawanie i usuwanie odcinków. Działa z arkuszami obliczeniowymi
`Przepływy` oraz `IS Solver`.

## Pobieranie

**[Pobierz HydroFlow.zip](https://github.com/JiMmpka/HydroFlow_Release/releases/download/Release/HydroFlow.zip)** — zawsze aktualna wersja.

Strona wydania: https://github.com/JiMmpka/HydroFlow_Release/releases/latest

## Wymagania

- Windows, Microsoft Excel 2016 lub nowszy / Microsoft 365 (32- lub 64-bitowy).
- Dostęp do internetu przy logowaniu. Po zalogowaniu dodatek działa także
  bez internetu do 3 dni.
- Konto (firmowy adres e-mail) dodane przez administratora.

## Instalacja

1. Pobierz `HydroFlow.zip`.
2. Rozpakuj **cały folder `HydroFlow`** w stałe miejsce na dysku (np.
   `Dokumenty\HydroFlow`). W środku są `HydroFlow.xlam` i folder `bin`.
   - **Folder `bin` musi zawsze leżeć obok `HydroFlow.xlam`** — bez niego
     dodatek nie działa.
   - Nie zmieniaj nazw plików w folderze `bin`.
3. W Excelu: **Plik → Opcje → Dodatki** → na dole **Zarządzaj: Dodatki
   programu Excel → Przejdź…** → **Przeglądaj…** → wskaż `HydroFlow.xlam` →
   upewnij się, że dodatek jest zaznaczony → **OK**.

Po instalacji w Excelu pojawia się karta wstążki **Flows**.

**Jeśli dodatek się nie wczytuje albo Excel blokuje jego makra** — Windows
mógł oznaczyć pobrany plik jako pochodzący z internetu. Zwykle nie jest to
potrzebne, ale w takiej sytuacji kliknij prawym przyciskiem plik ZIP (przed
rozpakowaniem) albo `HydroFlow.xlam` → **Właściwości** → zaznacz
**Odblokuj** (jeśli opcja jest dostępna) → **OK**, a potem uruchom Excel
ponownie.

## Pierwsze użycie — logowanie

Przy pierwszym obliczeniu dodatek poprosi o firmowy adres e-mail i wyśle na
niego kod. Wpisz kod z wiadomości — dalej dodatek pamięta logowanie i sam je
co jakiś czas odświeża. Ponowne logowanie może być potrzebne po dłuższym
czasie bez internetu albo po aktualizacji dodatku do nowej wersji.

Jeśli pojawi się komunikat o braku dostępu — skontaktuj się z administratorem.

## Używanie

Przyciski i skróty działają na arkuszu `Przepływy` albo `IS Solver`.

| Przycisk na karcie Flows | Skrót | Działanie |
|---|---|---|
| Oblicz przepływ | Ctrl+W | Oblicza przepływ dla przyjętych wymiarów i spadków |
| Oblicz przepływ z doborem wymiarów kanałów | Ctrl+K | Dobiera średnice kolektorów (dla rowów szerokość) bez zmiany spadków |
| Oblicz przepływ z doborem wymiarów kanałów i spadków | Ctrl+I | Dobiera średnice kolektorów dla spadków minimalnych |
| Dodaj odcinek | Ctrl+Q | Dodaje odcinek poniżej wskazanego (zaznacz nazwę odcinka w kolumnie A) |
| Usuń odcinek | Ctrl+E | Usuwa wskazany odcinek (zaznacz nazwę odcinka w kolumnie A) |

## Aktualizacja

1. Pobierz nowy `HydroFlow.zip`.
2. Zamknij Excel.
3. Zastąp zawartość folderu `HydroFlow` nowymi plikami (`HydroFlow.xlam` i
   cały folder `bin`).
4. Uruchom Excel — dodatek wczyta się z tego samego miejsca.

## Integralność pliku

W sekcji Assets wydania publikowany jest również `manifest.json` z numerem
wersji i sumą kontrolną SHA-256 pliku `HydroFlow.zip`. Suma pozwala wykryć
uszkodzony albo niezgodny plik.
