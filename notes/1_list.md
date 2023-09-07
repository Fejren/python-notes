### 1. Listy

Listy w Pythonie to struktury danych, które pozwalają przechowywać wiele wartości w jednej zmiennej. Możesz myśleć o liście jak o kontenerze, w którym możesz trzymać różne rzeczy, na przykład liczby, tekst czy inne zmienne.

Oto prosty przykład listy:

```python
moja_lista = [1, 2, 3, 4, 5]
```

W tym przypadku moja_lista to lista, która zawiera pięć liczb całkowitych. Możesz dodać, usunąć lub modyfikować elementy w liście. 
<br>Na przykład, aby dodać nowy element do listy, użyjemy metody append():

```python
moja_lista.append(6)
```

Możesz też odwoływać się do elementów listy po ich indeksach. Indeksy zaczynają się od 0. Na przykład, aby pobrać drugi element z listy, użyjemy `moja_lista[1]`, ponieważ 1 to indeks drugiego elementu.

Listy w Pythonie są elastyczne i mogą zawierać różne typy danych. Oto przykład listy, która zawiera różne rodzaje danych:

```python
dane = [1, "Hello", 3.14, True]
```

<hr>

### Operacje na listach

1. Dodawanie elementów do listy:
    * `append(element)`: Dodaje element na koniec listy.
    * `insert(index, element)`: Wstawia element na określonej pozycji.

```python
lista = [1, 2, 3]
lista.append(4)  # Dodaje 4 na koniec listy
lista.insert(1, 5)  # Wstawia 5 na drugiej pozycji (indeks 1)
```
2. Usunięcie elementów z listy:
    * `remove(element)`: Usuwa pierwsze wystąpienie określonego elementu.
    * `pop(index)`: Usuwa element na określonej pozycji i zwraca go (lub ostatni element, jeśli indeks nie jest podany).

```python
lista = [1, 2, 3, 4, 5]
lista.remove(3)  # Usuwa pierwsze wystąpienie 3
usuniety_element = lista.pop(1)  # Usuwa drugi element (indeks 1) i zwraca go
```

3. Operacje na indeksach
    * `lista[index]`: Pobiera element na określonej pozycji.
    * `lista[index] = nowy_element`: Modyfikuje element na określonej pozycji.

```python
lista = [1, 2, 3, 4, 5]
element = lista[2]  # Pobiera trzeci element (indeks 2)
lista[1] = 6  # Zmienia drugi element (indeks 1) na 6
```

4. Długość listy
    * `len(lista)`: Zwraca liczbę elementów w liście.

```python
lista = [1, 2, 3, 4, 5]
dlugosc = len(lista)  # Zwraca 5
```

5. Sortowanie i odwracanie
    * `lista.sort()`: Sortuje listę rosnąco.
    * `lista.sort(reverse=True)`: Sortuje listę malejąco.
    * `lista.reverse()`: Odwraca kolejność elementów w liście.

```python
lista = [3, 1, 4, 2, 5]
lista.sort()  # Sortuje rosnąco: [1, 2, 3, 4, 5]
lista.sort(reverse=True)  # Sortuje malejąco: [5, 4, 3, 2, 1]
lista.reverse()  # Odwraca: [1, 2, 3, 4, 5]
```

6. Sprawdzanie obecności elementu:
    * `element in lista`: Zwraca True, jeśli element jest w liście, w przeciwnym razie False

```python
lista = [1, 2, 3, 4, 5]
czy_jest_trzy = 3 in lista  # Zwraca True
czy_jest_szesnascie = 16 in lista  # Zwraca False
```

<hr>