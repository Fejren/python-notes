### 1. Listy

Listy w Pythonie to struktury danych, które pozwalają przechowywać wiele wartości w jednej zmiennej. Możesz myśleć o liście jak o kontenerze, w którym możesz trzymać różne rzeczy, na przykład liczby, tekst czy inne zmienne.

Oto prosty przykład listy:

```python
my_list = [1, 2, 3, 4, 5]
```

W tym przypadku my_list to lista, która zawiera pięć liczb całkowitych. Możesz dodać, usunąć lub modyfikować elementy w liście. 
<br>Na przykład, aby dodać nowy element do listy, użyjemy metody append():

```python
my_list.append(6)
```

Możesz też odwoływać się do elementów listy po ich indeksach. Indeksy zaczynają się od 0. Na przykład, aby pobrać drugi element z listy, użyjemy `my_list[1]`, ponieważ 1 to indeks drugiego elementu.

Listy w Pythonie są elastyczne i mogą zawierać różne typy danych. Oto przykład listy, która zawiera różne rodzaje danych:

```python
data = (1, "Hello", 3.14, True)
```

<hr>

### Operacje na listach

1. Dodawanie elementów do listy:
    * `append(element)`: Dodaje element na koniec listy.
    * `insert(index, element)`: Wstawia element na określonej pozycji.

```python
my_list = [1, 2, 3]
my_list.append(4)  # Dodaje 4 na koniec listy
my_list.insert(1, 5)  # Wstawia 5 na drugiej pozycji (indeks 1)
```
2. Usunięcie elementów z listy:
    * `remove(element)`: Usuwa pierwsze wystąpienie określonego elementu.
    * `pop(index)`: Usuwa element na określonej pozycji i zwraca go (lub ostatni element, jeśli indeks nie jest podany).

```python
my_list = [1, 2, 3, 4, 5]
my_list.remove(3)  # Usuwa pierwsze wystąpienie 3
removed_element = my_list.pop(1)  # Usuwa drugi element (indeks 1) i zwraca go
```

3. Operacje na indeksach
    * `my_list[index]`: Pobiera element na określonej pozycji.
    * `my_list[index] = nowy_element`: Modyfikuje element na określonej pozycji.

```python
my_list = [1, 2, 3, 4, 5]
element = my_list[2]  # Pobiera trzeci element (indeks 2)
my_list[1] = 6  # Zmienia drugi element (indeks 1) na 6
```

4. Długość listy
    * `len(my_list)`: Zwraca liczbę elementów w liście.

```python
my_list = [1, 2, 3, 4, 5]
length = len(my_list)  # Zwraca 5
```

5. Sortowanie i odwracanie
    * `my_list.sort()`: Sortuje listę rosnąco.
    * `my_list.sort(reverse=True)`: Sortuje listę malejąco.
    * `my_list.reverse()`: Odwraca kolejność elementów w liście.

```python
my_list = [3, 1, 4, 2, 5]
my_list.sort()  # Sortuje rosnąco: [1, 2, 3, 4, 5]
my_list.sort(reverse=True)  # Sortuje malejąco: [5, 4, 3, 2, 1]
my_list.reverse()  # Odwraca: [1, 2, 3, 4, 5]
```

6. Sprawdzanie obecności elementu:
    * `element in my_list`: Zwraca True, jeśli element jest w liście, w przeciwnym razie False

```python
my_list = [1, 2, 3, 4, 5]
is_3_in_list = 3 in my_list  # Zwraca True
is_16_in_list = 16 in my_list  # Zwraca False
```

<hr>