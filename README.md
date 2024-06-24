```mermaid
graph TD
    A[Kontrola surowca przed zasypem] -->|Dane surowca| B[Magazyn danych: Etykieta surowca]
    A -->|Numer serii| C[Magazyn danych: Karta serii]

    D[Kontrola parametrów linii produkcyjnej] -->|Parametry procesu| C
    E[Kontrola wyglądu profilu gotowego] -->|Wzorzec koloru| F[Magazyn danych: Wzorzec koloru]
    E -->|Instrukcja jakości| G[Magazyn danych: Instrukcja jakości]

    H[Kontrola oznakowania wyrobu gotowego] -->|Krajowa Deklaracja| I[Magazyn danych: Krajowa Deklaracja Właściwości Użytkowych]
    H -->|Oznakowanie| J[Magazyn danych: Oznakowanie zgodne z Krajową Oceną Techniczną]

    K[Kontrola wymiarów produktu gotowego] -->|Wymiary produktu| C
    L[Kontrola pakowania] -->|Instrukcja pakowania| M[Magazyn danych: Instrukcja pakowania]
    L -->|Arkusz pakowania| N[Magazyn danych: Arkusz "Pakowanie"]

    O[Kontrola wypełnienia dokumentacji jakościowej] -->|Formularze jakościowe| P[Magazyn danych: Formularze jakościowe]
    Q[Kontrola przed wysyłką] -->|Raport kontroli| R[Magazyn danych: Raport kontroli przed wysyłką]

