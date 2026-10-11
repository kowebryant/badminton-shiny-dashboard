# Badminton Data Dashboard 🏸

[![R](https://img.shields.io/badge/R-276DC3?logo=r&logoColor=white)](https://www.r-project.org/)
[![Shiny](https://img.shields.io/badge/Shiny-Web_App-blue?logo=rstudio&logoColor=white)](https://shiny.rstudio.com/)
[![ggplot2](https://img.shields.io/badge/ggplot2-Data_Viz-orange)](https://ggplot2.tidyverse.org/)

## 📌 Opis projektu
Interaktywna aplikacja webowa (Dashboard) stworzona w języku R przy użyciu frameworka **Shiny**. Projekt ma na celu kompleksową analizę i wizualizację danych dotyczących polskiego badmintona (ewidencja zawodników i sędziów) oraz danych historycznych z Igrzysk Olimpijskich.

## 🛠️ Wykorzystane technologie
* **Język:** R
* **Framework:** Shiny
* **Przetwarzanie danych:** `dplyr`, `tidyr`, `stringr`, `readxl`
* **Wizualizacja i GIS:** `ggplot2`, `ggiraph` (interaktywne wykresy), `sf`, `geodata` (mapowanie przestrzenne)

## 📊 Główne funkcjonalności
1. **Interaktywna mapa Polski (GIS):** 
   * Dynamiczne wyświetlanie zagęszczenia zawodników i sędziów z podziałem na województwa.
   * Obliczanie wskaźników (np. liczba zawodników z licencją przypadająca na jednego sędziego).
   * Interaktywność (hover, tooltipy) zrealizowana za pomocą pakietu `ggiraph`.
2. **Zaawansowane filtrowanie danych:** 
   * Analiza demograficzna i kategoryzacyjna: podział zawodników na kategorie wiekowe (od U9 po Elitę) oraz sędziów ze względu na posiadane uprawnienia i ważność licencji.
3. **Analiza Danych Olimpijskich:**
   * Wizualizacja trendów w czasie (liczba zawodników z podziałem na płeć).
   * Generowanie podiów medalistów.
   * Analiza cech fizycznych (np. rozkład wzrostu zawodników z poszczególnych krajów za pomocą wykresów pudełkowych / boxplots).

## 🗂️ Struktura danych i czyszczenie
W projekcie zaimplementowano zaawansowane skrypty parsujące surowe pliki Excela (m.in. dynamiczne pętle wyodrębniające tabele sędziów z nieustandaryzowanych bloków tekstu) oraz ujednolicono nazewnictwo i systemy referencyjne dla regionów geograficznych.