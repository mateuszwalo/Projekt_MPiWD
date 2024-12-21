# 🌍 Analiza katastrof globalnych - zaliczenie przedmiotu Metody Pozyskiwania i Wizualizacji danych

Witaj w projekcie dotyczącym analizy katastrof na całym świecie. Celem tego projektu jest analiza danych związanych z globalnymi katastrofami, wykorzystanie różnych modeli maszynowego uczenia (w tym regresji logistycznej, lasu losowego i drzewa decyzyjnego) oraz ocena ich wydajności w przewidywaniu rodzaju katastrofy na podstawie dostępnych predyktorów.

## 📂 Zawartość repozytorium

- `Analiza_katastrof_globalnych.qmd` – Główny plik Quarto, w którym przeprowadzona jest analiza.
- `Analiza_katastrof_globalnych.html` – Wygenerowany raport HTML z analizy -> polecam otwierać za pomocą githacka
- `train_balanced.csv` – Zbalansowane dane treningowe po zastosowaniu SMOTE.
- `test_data.csv` – Dane testowe do oceny modelu.
- `final_data.csv` – Ostateczny zestaw danych używanych w analizach.
- `simplified_data.csv` – Uproszczony zestaw danych do szybszej analizy.
- `public_emdat_custom_request_2024-10-03_fdbbae24-da6c-4137-b8d4-3c5548a622df.xlsx` – Pierwowzór danych pobranych przez API

## 📊 Modele

W ramach tego projektu używane są różne techniki modelowania:

- **Regresja logistyczna** – prosta, ale skuteczna metoda klasyfikacji.
- **Drzewo decyzyjne** – zaawansowana metoda klasyfikacji z wykorzystaniem struktury drzewa.
- **Las losowy** – zbiór drzew decyzyjnych do poprawy dokładności modelu.

Modele te są trenowane na danych zawierających informacje o różnych katastrofach, takich jak ich typy, regiony, liczba ofiar oraz inne zmienne. Celem jest stworzenie modelu, który będzie w stanie przewidywać rodzaj katastrofy na podstawie dostępnych informacji.

## 📈 Wykresy i analizy

W projekcie znajdziesz interaktywne wykresy i analizy, w tym:

- **Krzywe ROC** – ocena wydajności modeli przy różnych progach decyzyjnych.
- **Porównanie modeli** – zestawienie wyników różnych algorytmów na podstawie miar takich jak dokładność (accuracy) i AUC.
- **Drzewo decyzyjne** – wizualizacja drzewa decyzyjnego po zastosowaniu algorytmu SMOTE do balansowania danych.

## 🚀 Uruchomienie projektu

Aby uruchomić projekt, wykonaj poniższe kroki:

1. **Zainstaluj wymagane pakiety** w R:

    ```r
    install.packages(c("caret", "randomForest", "rpart", "pROC", "ggplot2", "dplyr", "quarto"))
    ```

2. **Załaduj dane**:

    Wczytaj odpowiednie dane, np. `train_balanced.csv` i `test_data.csv`, za pomocą poniższego kodu:

    ```r
    train_balanced <- read.csv("train_balanced.csv")
    test_data <- read.csv("test_data.csv")
    ```

3. **Uruchom skrypt w R**:

    Skorzystaj z pliku Quarto (`Analiza_katastrof_globalnych.qmd`), aby uruchomić analizę i wygenerować raport. Jeśli używasz Quarto, wystarczy wykonać poniższą komendę:

    ```bash
    quarto render Analiza_katastrof_globalnych.qmd
    ```

4. **Zobacz wyniki**:

    Wygenerowany raport HTML (`Analiza_katastrof_globalnych.html`) zawiera wszystkie wyniki analizy, wykresy i porównania modeli.

## 📚 Wymagania

- R w wersji 4.0 lub wyższej
- Quarto
- Pakiety: `caret`, `randomForest`, `rpart`, `pROC`, `ggplot2`, `dplyr`

## 🎯 Cele projektu

1. **Analiza skuteczności modeli** – porównanie różnych algorytmów (regresja logistyczna, las losowy, drzewo decyzyjne).
2. **Przewidywanie katastrof** – stworzenie modelu, który pomoże w przewidywaniu typu katastrofy na podstawie dostępnych danych.
3. **Wizualizacja wyników** – stworzenie interaktywnych wykresów dla lepszego zrozumienia wyników.

## 📄 Licencja

Ten projekt jest licencjonowany na zasadach [MIT License](LICENSE).

## 💬 Kontakt

Masz pytania? Chcesz dowiedzieć się więcej? Skontaktuj się ze mną!

- E-mail: [mateusz.walo@datascience.com](mailto:mateusz.walo@datascience.com)
  
Dziękuję za odwiedzenie mojego repozytorium! 😊
