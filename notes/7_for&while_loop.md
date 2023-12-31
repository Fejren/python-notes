### 7. Pętle for i while
Pętle są używane do wielokrotnego wykonania określonego fragmentu kodu. 

### Pętla for
Pętla for jest używana, gdy chcemy iterować przez sekwencję (taką jak lista, krotka, napis, itp.) i wykonywać określone operacje dla każdego elementu w tej sekwencji.

Składnia pętli for
```python
lista = [1, 2, 3, 4, 5]
for element in lista:
    # Wykonaj operacje na elemencie
    print(element)
```

Pętle instrukcje w pętli można wykonać określoną liczbę razy np. <br>
<b>range(start, stop[, krok])</b>
```python
n = 5
for i in range(5):
    print(i) # Wypisze 0, 1, 2, 3, 4
```

```python
for i in range(2, 5):
    print(i) # Wypisze 2, 3, 4
```

```python
# zaczyna od 0 kończy na 10 elemencie, wypisuje co drugi element
for x in range(0, 10, 2):
  print(x) # Wypisze liczby parzyste od 0 do 9
```

Pętlę można zapisać w jednej linii
```python
liczby = [1, 2, 3, 4, 6]

[print(liczba) for liczba in liczby]

# Również można dodać warunek do pętli oraz jej wynik przypisać do zmiennej
liczba = [i for i in liczby if i == 2]
print(liczba) # Wypisze 2
```

### Pętla while
Pętla while jest używana, gdy chcemy wykonywać określony blok kodu, dopóki pewien warunek jest spełniony. 

Składnia pętli while
```python
while warunek:
    # Wykonaj operacje dopóki warunek jest prawdziwy
    print("To jest pętla while")
```

Przykład użycia
```python
counter = 1
while counter <= 5: # Gdy counter będzie równy 5 pętla przerwie swoje działanie
    print(counter)
    counter += 1
```

Pętlę można zapisać w jednej linii

```python
while True: print("something") # Będzie wypisywać w nieskończoność "something"
```
Inny przykład
```python
counter = 0
# Dodatkowe operacje oddzielamy ;
while counter <= 5: print("something");counter += 1; print("else") 
```

<hr>