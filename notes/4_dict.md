### 4. Słownik

Słownik (ang. dictionary) w Pythonie to specjalny rodzaj struktury danych, która pozwala przechowywać pary klucz-wartość. Klucz jest unikalny w danym słowniku i jest używany do odnalezienia odpowiadającej mu wartości. Można sobie to wyobrazić jak książkę, gdzie klucz to jest hasło, a wartość to definicja.

Oto przykład słownika w Pythonie:

```python
my_dict = {"jabłko": "owoc", "kot": "zwierzę", "samochód": "pojazd"}
```

W tym przykładzie mamy słownik, który zawiera trzy pary klucz-wartość:

* Klucz "jabłko" ma wartość "owoc".
* Klucz "kot" ma wartość "zwierzę".
* Klucz "samochód" ma wartość "pojazd".

Możemy teraz użyć klucza, aby uzyskać odpowiadającą mu wartość:
```python
print(my_dict["kot"])  # Wyświetli "zwierzę"
```

Dane mogą być też bardziej złożone

```python
user_data = {
    "name": "Dawid",
    "age": 19,
    "cars": [ # Jako wartość w słowniku można użyć listę
        "Seat Ibiza 6j",
        "Nissan 370Z"
    ],
}

# Sprawdzanie długości słownika
print(len(user_data)) # Wyświetli 3, ponieważ taka jest liczba kluczy
```

Słowniki są bardzo przydatne, gdy chcemy przechowywać dane, które mają jakieś powiązania między sobą. Możemy je używać do przechowywania informacji, takich jak tłumaczenia słów w słowniku, dane osobowe w bazie danych czy parametry konfiguracyjne w programie.

<hr>