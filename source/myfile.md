Wersja dokumentu
----------------
Dokument w wersji 1.0-alpha

Wprowadzone zmiany
===================

Dodano dokumentację.
Dodane opis projektu, wymagania funkcjonalne i niefunkcjonalne.

Spis Treści
============

Opis projektu
==============
Założeniem projektu jest inteligentne sterowanie oświetleniem w pokoju na podstawie odczytów z czujnika temperatury oraz czujnika natężenia światła. W momencie naciśnięcia przycisku włączania oświetlenia odczytywane jest natężenie światła oraz temperatura. W przypadku niskiej jasności włączane jest oświetlenie pokoju. W zależności od odczytanej temperatury uruchomiona jest wybrana żarówka. W przypadku niskiej temperatury włączana jest żarówka o ciepłej barwie światła. W przypadku wysokiej temperatury włączana jest żarówka o zimnej barwie światła. W przypadku wysokiej jasności i wyłączonego światła światło nie zostaje włączone. W przypadku włączonego światła i wciśnięcia przycisku światło zostaje wyłączone. Mikrokontroler dokonuje pomiarów co 10 sekund aby wykryć konieczność zmiany barwy światła, tylko przy włączonym świetle.

Wymagania
=========

Wymagania funkcjonalne
----------------------

1. Mikrokontroler dokonuje pomiarów co 10 sekund, przy włączonym świetle.
2. Po wykryciu zmiany temperatury jest włączana odpowiednia żarówka.
3. Odczyt z fotorezystora wartości poniżej 400 uznajemy jako ciemno, a wartości powyżej 400 uznajemy jako jasno.

Wymagania niefunkcjonalne
--------------------------

1. Światło zostaje włączone kiedy wciśnięty zostanie przycisk a światło jest wyłączone i jest ciemno.
2. Światło zostaje wyłączone kiedy wciśnięty zostanie przycisk a światło jest włączone.
3. Światło pozostaje wyłączone kiedy w pomieszczeniu jest jasno, a zostanie wciśnięty przycisk.
4. Żarówka o ciepłej barwie światła jest włączona, kiedy jest zimno.
5. Żarówka o zimnej barwie światła jest włączona, kiedy jest ciepło.
