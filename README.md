# 🌍 Analiza katastrof globalnych

Witaj w projekcie dotyczącym analizy katastrof na całym świecie. Celem tego projektu jest analiza danych związanych z globalnymi katastrofami, wykorzystanie różnych modeli maszynowego uczenia (w tym regresji logistycznej, lasu losowego i drzewa decyzyjnego) oraz ocena ich wydajności w przewidywaniu rodzaju katastrofy na podstawie dostępnych predyktorów.

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

## 📂 Pliki

W projekcie znajdują się następujące pliki:

- `train_balanced.csv` – zbalansowane dane treningowe po zastosowaniu SMOTE.
- `test_data.csv` – dane testowe.
- Pliki skryptów R (np. `model_analysis.R`) do przeprowadzania analizy oraz trenowania modeli.

## 🚀 Uruchomienie projektu

Aby uruchomić projekt, wykonaj poniższe kroki:

1. **Zainstaluj wymagane pakiety** w R:

    ```r
    install.packages(c("caret", "randomForest", "rpart", "pROC", "ggplot2", "dplyr"))
    ```

2. **Załaduj dane** (np. `train_balanced.csv` i `test_data.csv`) i rozpocznij analizę w R.

3. **Uruchom skrypt** w R, aby przetrenować modele i wygenerować wykresy.

## 📚 Wymagania

- R w wersji 4.0 lub wyższej
- Pakiety: `caret`, `randomForest`, `rpart`, `pROC`, `ggplot2`, `dplyr`
- Środowisko do pracy z Quarto (jeśli chcesz wygenerować raporty HTML)

## 🎯 Cele projektu

1. **Analiza skuteczności modeli** – porównanie różnych algorytmów (regresja logistyczna, las losowy, drzewo decyzyjne).
2. **Przewidywanie katastrof** – stworzenie modelu, który pomoże w przewidywaniu typu katastrofy na podstawie dostępnych danych.
3. **Wizualizacja wyników** – stworzenie interaktywnych wykresów dla lepszego zrozumienia wyników.

## 📄 Licencja

Ten projekt jest licencjonowany na zasadach [MIT License](LICENSE).

## 💬 Kontakt

Masz pytania? Chcesz dowiedzieć się więcej? Skontaktuj się ze mną!

- E-mail: [mateusz.walo@example.com](mailto:mateusz.walo@example.com)
- GitHub: [@mateusz-walo](https://github.com/mateusz-walo)

Dziękuję za odwiedzenie mojego repozytorium! 😊
