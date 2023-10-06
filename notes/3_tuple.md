### 3. Tuple

Tupla znana też jako krotka w Pythonie to rodzaj kolekcji, która przechowuje różne elementy, ale jest niemutowalna, co oznacza, że nie możesz zmieniać jej zawartości po jej utworzeniu. Każdy element w tupli ma swoją pozycję, a te pozycje są numerowane od zera.

Oto kilka prostych przykładów:

1. Tworzenie tupli:

```python
my_tuple = (1, 2, 3)
```

Tuple w Pythonie są elastyczne i mogą zawierać różne typy danych. Oto przykład tupli, która zawiera różne rodzaje danych:

```python
data = [1, "Hello", 3.14, True]
```

2. Indeksowanie tupli:

Możesz uzyskać dostęp do elementów tupli za pomocą indeksów (numerów pozycji) w nawiasach kwadratowych:
```python
first_element = my_tuple[0]  # Pobiera pierwszy element (1)
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

Tupla może być używana jako klucz w słowniku, ponieważ jest niemutowalna i haszowalna. <br>
Tuple są haszowalne (hashable), co oznacza, że mają stały i niezmienny identyfikator (hasz), który jest używany przez słownik do szybkiego dostępu do wartości.
Na przykład:
```python
my_tuple = (1, 2)
dictionary = {my_tuple: "value"}

print(dictionary[my_tuple]) # Wypisze: value
```
<hr>

### Kluczowe różnice między tuplą a listą

1. Wydajność
    * Tuple są znacznie szybsze podczas obliczeń niż listy.
    * https://stackoverflow.com/questions/68630/are-tuples-more-efficient-than-lists-in-python

2. Nie muszą być kopiowane
   ```python
   a = (10, 20, 30)
   b = tuple(a)
   a is b # True
   ```
   W kontraście do list
   ```python
   a = [10, 20, 30]
   b = list(a)
   a is b # False
   ```
3. Tuple nie tworzą nadmiarowej alokacji w pamięci
   ```python
   import sys
   # Tupla
   sys.getsizeof(tuple(iter(range(10)))) # Wynik to: 128
   # Lista
   sys.getsizeof(list(iter(range(10)))) # Wynik to: 200
   ```

4. Tuple odnoszą się bezpośrednio do swoich elementów

   Tupla są jak paczka, która trzyma różne rzeczy razem. Możesz się do tego odnieść bezpośrednio, jakbyś wiedział, że coś jest w paczce i możesz to z niej wyjąć.
   
   Natomiast listy zamiast trzymać same rzeczy, trzymają one wskazówki (adresy) do tych rzeczy. I potem musisz udać się pod wskazany adres.
   
   Dlatego krotki są szybsze, jeśli chodzi o znajdowanie i wyciąganie rzeczy, ponieważ wszystko jest bezpośrednio w paczce, podczas gdy w przypadku list, musisz znaleźć pudełko, zanim znajdziesz rzeczy w środku.

   <br>
   
   Dowód:
   ```python
   # Wyszukiwanie po indexie
   $ python -m timeit -s 'a = (10, 20, 30)' 'a[1]' # Tupla
   10000000 loops, best of 3: 0.0304 usec per loop
   $ python -m timeit -s 'a = [10, 20, 30]' 'a[1]' # Lista
   10000000 loops, best of 3: 0.0309 usec per loop
   
   # Pobieranie wartości do zmiennych
   $ python -m timeit -s 'a = (10, 20, 30)' 'x, y, z = a' # Tupla
   10000000 loops, best of 3: 0.0249 usec per loop
   $ python -m timeit -s 'a = [10, 20, 30]' 'x, y, z = a' # Lista
   10000000 loops, best of 3: 0.0251 usec per loop
   ```
   
<hr>