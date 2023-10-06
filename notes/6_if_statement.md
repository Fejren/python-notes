### 6. Instrukcja warunkowa 'if'

If jest używane jako instrukcja warunkowa, która pozwala na wykonanie określonych bloków kodu tylko wtedy, gdy określony warunek jest spełniony (prawdziwy).

<br> Składnia if wygląda następująco:

```python
if warunek:
    # Kod do wykonania, jeśli warunek jest prawdziwy
else:
    # Kod do wykonania, jeśli warunek nie jest prawdziwy
```

Praktyczny przykład

```python
age = 18
if age >= 18:
    print("Jesteś pełnoletni")
else:
    print("Jesteś niepełnoletni")
```

If można zapisać również w nieco innej formie
```python
wykonaj_jeżeli_prawda if warunek == True else wykonaj_jeżeli_fałsz
# Przykład
print("Jesteś pełnoletni") if age >= 18 else print("Jesteś niepełnoletni")
```

<hr>
