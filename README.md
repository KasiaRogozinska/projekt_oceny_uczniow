# Przewidywanie ocen uczniów - projekt Machine Learning

## Opis danych
Zbiór danych pochodzi z UCI Machine Learning Repository i dotyczy wyników uczniów dwóch portugalskich szkół średnich.
- Liczba obserwacji: 395 uczniów
- Liczba cech: 33 (dane demograficzne, rodzinne i szkolne)
- Źródło: https://archive.ics.uci.edu/ml/datasets/Student+Performance

## Cel analizy
Celem projektu jest przewidywanie końcowej oceny ucznia (G3) na podstawie mierzalnych parametrów stylu życia i historii edukacyjnej. 

## Zakres analizy
- Wizualizacja danych i analiza korelacji
- Czyszczenie i przygotowanie danych
- Feature engineering (G_avg, studytime_per_grade, absences_per_studytime)
- Implementacja i porównanie dwóch modeli regresji
- Optymalizacja hiperparametrów (GridSearchCV)

## Modele
- Regresja Liniowa
- Las Losowy (Random Forest) z GridSearchCV

## Wyniki
| Model | RMSE (zbiór testowy) |
| Regresja Liniowa | 0.4579 |
| Las Losowy (GridSearchCV) | 0.5302 |

Lepszym modelem okazała się Regresja Liniowa (RMSE = 0.4579).
Wynik ten może wynikać z małego rozmiaru zbioru danych oraz dyskretnego charakteru zmiennej docelowej (6 wartości w skali 1-6).
