# Dane przestrzenne w uczeniu maszynowym

To repozytorium zawiera materiały do warsztatu "**Dane przestrzenne w uczeniu maszynowym - środowisko R**" przeprowadzonego podczas konferencji [Geoinformacja: Nauka – Praktyka – Edukacja](https://geoinformacja20uam.pl/) (02.12.2022 r.).

**R** jest jednym z najbardziej popularnych języków programowania używanych do analizy danych.
**R** znalazł szczególne zastosowanie w takich dziedzinach jak ekologia, leśnictwo, hydrologia czy teledetekcja dzięki swojej prostocie, możliwości automatyzacji powtarzalnych zadań oraz ogromnemu wsparciu przez jego społeczność.
**R** stanowi świetną alternatywę dla standardowych aplikacji GIS znacząco rozszerzając ich możliwość w kontekście statystycznej analizy danych i uczenia maszynowego.

## Wymagania

Warsztat skierowany jest do osób, które posiadają podstawową wiedzę i doświadczenie w środowisku **R**.
Wymagana jest również podstawowa wiedza z zakresu GIS oraz teledetekcji satelitarnej.

Jeśli jesteś osobą początkującą i chcesz rozszerzyć (lub odnowić) swoją wiedzę odnośnie środowiska **R**, to polecam bezpłatny kurs online "[Pogromcy Danych](http://pogromcydanych.icm.edu.pl/)" przygotowany przez Uniwersytet Warszawski.
Dostępny jest również podręcznik w języku polskim: "[Elementarz programisty: Wstęp do programowania używając R](https://jakubnowosad.com/elp/)".

Kolejne podręczniki (w języku angielskim) dotyczące przestrzennej analizy danych to:

- [**Spatial Data Science with R and “terra”**](https://rspatial.org/terra/)
- [Geocomputation with R](https://geocompr.robinlovelace.net/)
- [Spatial Data Science, with applications in R](https://r-spatial.org/book/)

## Wstęp

**1. Instalacja R**

**R** jest językiem programowania.
Można go pobrać dla [Windows](https://cloud.r-project.org/bin/windows/base/R-4.2.2-win.exe), [MacOS](https://cloud.r-project.org/bin/macosx/) oraz [Linux](https://cloud.r-project.org/bin/linux/).

**2. Instalacja RStudio**

**RStudio** natomiast jest zintegrowanym środowiskiem programistycznym z edytorem kodu.
Aplikacja dostępna jest również na różnych platformach do pobrania w [tym miejscu](https://posit.co/download/rstudio-desktop/).

**3. Instalacja pakietów**

Jednym z najpopularniejszych pakietów do analizy przestrzennej w R jest pakiet [**terra**](https://github.com/rspatial/terra).
Umożliwia on analizę zarówno danych rastrowych i wektorowych.
Można go zainstalować w następujący sposób:

```r
install.packages("terra")
```

Następnie można go załadować używając funkcji `library()`.

```r
library("terra")
```

Dokumentację do tego pakietu znajdziesz tutaj: <https://rspatial.github.io/terra/reference/terra-package.html>

## Materiały &#128681;

Niezbędne dane rastrowe (scena Landsat 8, klasyfikacja pokrycia terenu) oraz wektorowe znajdziesz na [Dysku Google](https://drive.google.com/file/d/1WfAYCd42nLoEhpyICJxoVOaGR-t1Jcdj/view) oraz [Zenodo](https://zenodo.org/record/7299645).
Po pobraniu dane należy rozpakować.

Interaktywne zeszyty (*.Rmd*) oraz statyczne dokumenty (*.html*) możesz pobrać z repozytorium [https://github.com/kadyb/GEOINF2022](https://github.com/kadyb/GEOINF2022):

1. [Klasyfikacja nienadzorowana](https://kadyb.github.io/GEOINF2022/Grupowanie.html)
2. [Klasyfikacja nadzorowana](https://kadyb.github.io/GEOINF2022/Klasyfikacja.html)
3. [Zadanie](https://kadyb.github.io/GEOINF2022/Zadanie.html)

Opis kanałów spektralnych znajdziesz [tutaj](https://landsat.gsfc.nasa.gov/satellites/landsat-8/landsat-8-bands/).
Informacje o klasach pokrycia terenu Sentinel-2 Global Land Cover (S2GLC) znajdziesz [tutaj](https://s2glc.cbk.waw.pl/extension).

## Kontakt

Jeśli masz jakieś pytania albo potrzebujesz pomocy, napisz do mnie pod adres krzysztof.dyba@amu.edu.pl.
