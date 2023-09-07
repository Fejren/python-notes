### 2. Zbiory

Zbiory w Pythonie są kolekcją elementów, ale w przeciwieństwie do list, nie mogą zawierać duplikatów. To znaczy, że w zbiorze nie ma dwóch identycznych elementów. Zbiory są przydatne, gdy chcemy przechowywać unikalne wartości i wykonywać na nich operacje takie jak sprawdzanie, czy element jest w zbiorze, dodawanie i usuwanie elementów.

Oto kilka przykładów zastosowania zbiorów w Pythonie:

1. Usuwanie duplikatów z listy:

```python
lista = [1, 2, 2, 3, 4, 4, 5]
zbior = set(lista)
unikalne_elementy = list(zbior)
print(unikalne_elementy) # wynik: [1, 2, 3, 4, 5]
```

2. Sprawdzanie czy element jest w zbiorze:

Możemy użyć operatora in do sprawdzenia, czy dany element znajduje się w zbiorze. Na przykład:

```python
zbior = {1, 2, 3, 4, 5}
if 3 in zbior:
    print("3 jest w zbiorze")
else:
    print("3 nie jest w zbiorze")
    
# wynik: 3 jest w zbiorze
```

3. Operacje na zbiorach:

Zbiory pozwalają wykonywać różne operacje takie jak unia, przecięcie, różnica itp. Przykład:
```python
zbior_A = {1, 2, 3, 4}
zbior_B = {3, 4, 5, 6}

unia = zbior_A | zbior_B
przeciecie = zbior_A & zbior_B
roznica = zbior_A - zbior_B

print("Unia:", unia)
print("Przecięcie:", przeciecie)
print("Różnica:", roznica)

# Unia: {1, 2, 3, 4, 5, 6}
# Przecięcie: {3, 4}
# Różnica: {1, 2}
```

<hr>