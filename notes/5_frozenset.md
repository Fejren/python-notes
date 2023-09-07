### 5. Frozenset

`frozenset` jest przydatny, gdy chcemy stworzyć zbiór, który nie będzie podatny na zmiany, na przykład jako klucz w słowniku, ponieważ klucze w słowniku muszą być niemutowalne.

```python
# Tworzymy zwykły zbiór (set)
zwykly_zbior = {1, 2, 3}

# Możemy dodać nowy element do zwykłego zbioru
zwykly_zbior.add(4)
print(zwykly_zbior)  # Wynik: {1, 2, 3, 4}

# Teraz utwórzmy frozenset
niezmienialny_zbior = frozenset([1, 2, 3])

# Nie możemy dodać nowego elementu do frozenset
# To spowoduje błąd: 'frozenset' object has no attribute 'add'
# niezmienialny_zbior.add(4)

# Nie możemy też usuwać elementów
# To spowoduje błąd: 'frozenset' object has no attribute 'remove'
# niezmienialny_zbior.remove(1)
```

<hr>