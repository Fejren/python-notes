### 3. Tuple

Tuple w Pythonie to rodzaj kolekcji, która przechowuje różne elementy, ale jest niemutowalna, co oznacza, że nie możesz zmieniać jej zawartości po jej utworzeniu. Każdy element w tupli ma swoją pozycję, a te pozycje są numerowane od zera.

Oto kilka prostych przykładów:

1. Tworzenie tupli:

```python
moja_tupla = (1, 2, 3)
```

2. Indeksowanie tupli:

Możesz uzyskać dostęp do elementów tupli za pomocą indeksów (numerów pozycji) w nawiasach kwadratowych:
```python
pierwszy_element = moja_tupla[0]  # Pobiera pierwszy element (1)
```

3. Tupla jako niezmienialna:

Nie możesz zmieniać elementów w tupli po jej utworzeniu. Poniższy kod spowoduje błąd:
```python
moja_tupla[0] = 4  # To wywoła błąd, bo tupla jest niemutowalna
```

4. Rozpakowanie tupli

Możesz rozpakować elementy tupli do zmiennych w jednej linii:
```python
a, b, c = moja_tupla
# Teraz a = 1, b = 2, c = 3
```

5. Tupla jako klucz w słowniku:

Tupla może być używana jako klucz w słowniku, ponieważ jest niemutowalna. Na przykład:
```python
slownik = {(1, 2): "wartość"}
```

Tupla jest przydatnym typem danych w Pythonie, gdy chcesz zachować zestaw elementów, które nie powinny być zmieniane po utworzeniu.

<hr>