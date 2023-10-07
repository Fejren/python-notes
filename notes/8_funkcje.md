### 8. Funkcje
Funkcje są blokami kodu, które wykonują określone zadania i mogą być wywoływane w różnych miejscach programu.
<br>Pozwalają na zorganizowanie kodu w bardziej czytelny i efektywny sposób oraz umożliwiają unikanie powtarzania się kodu poprzez wielokrotne wykorzystywanie tych samych instrukcji.

Struktura funkcji
* Struktura funkcji, która nic nie zwraca (void)
```python
def nazwa_funkcji(argumenty):
    # kod funkcji
    # ...
```

* Struktura funkcji, która coś zwraca
```python
def nazwa_funkcji(argumenty):
    # kod funkcji
    # ...
    return wynik
```

Przykłady:

```python
def add(a, b):
    result = a + b
    return result # zwracanie wyniku dodawania

# Wywołanie funkcji
sum = add(3, 5)
print(sum) # Wypisze: 8 
```

```python
def tell_me_something(something):
    print(something) # funkcja nic nie zwraca tylko wypisuje w konsoli
    
# Wywołanie funkcji
tell_me_something("Something") 
# Działa tak samo jak przykład wyżej
tell_me_something(something="Something") 
```

<hr>