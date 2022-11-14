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
Założeniem projektu jest automatyczne sterowanie oświetleniem w pokoju na podstawie odczytów z czujnika ruchu oraz czujnika natężenia światła. W momencie wykrycia ruchu odczytywane jest natężenie światła. W przypadku niskiej jasności włączane jest oświetlenie pokoju na 1 minutę. W przypadku wysokiej jasności oraz wyłączonego światła w pokoju światło nie zostaje włączone. Mikrokontroler dokonuje pomiarów co 10 sekund aby wykryć konieczność pozostawienia włączonego światła.

Wymagania
=========

Wymagania funkcjonalne
----------------------

1. Mikrokontroler dokonuje pomiarów co 10 sekund.
2. Po wykryciu ruchu oświetlenie jest włączane na 1 minutę.
3. Odczyt z fotorezystora wartości poniżej 400 uznajemy jako ciemno, a wartości powyżej 400 uznajemy jako jasno.

Wymagania niefunkcjonalne
--------------------------

1. Światło zostaje włączone kiedy w pomieszczeniu jest ciemno i zostanie wykryty ruch.
2. Światło zostaje wyłączone kiedy w ciągu ostatniej minuty nie wykryto ruchu.
3. Światło pozostaje włączone kiedy w pomieszczeniu wykrywany jest ruch.
4. Światło pozostaje wyłączone kiedy w pomieszczeniu jest jasno, bez interpretowania odczytów czujnika ruchu.
