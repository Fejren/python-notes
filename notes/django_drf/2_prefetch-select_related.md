### 2. prefetch_related('lookup') i select_related('lookup')

<b>prefetch_related()</b> - zwraca QuerySet który automatycznie pobierze za jednym razem powiązane obiekty dla każdego z określonych wyszukiwań. <br>

Ma to podobny cel jak <i>select_related</i>, ponieważ oba mają na celu powstrzymanie zalewu zapytań do bazy danych spowodowanych dostępem do powiązanych obiektów, ale strategia jest zupełnie inna

### Zasada działania
Załóżmy na przykład, że są następujące modele:

```python
from django.db import models


class Topping(models.Model):
    name = models.CharField(max_length=30)


class Pizza(models.Model):
    name = models.CharField(max_length=50)
    toppings = models.ManyToManyField(Topping)

    def __str__(self):
        return "%s (%s)" % (
            self.name,
            ", ".join(topping.name for topping in self.toppings.all()),
        )
```

```python
>>> Pizza.objects.all()
["Hawaiian (ham, pineapple)", "Seafood (prawns, smoked salmon)"...
```
Problem polega na tym, że za każdym razem, gdy `Pizza.__str__()` to wykonuje `self.toppings.all()`,
musi wysłać zapytanie do bazy danych, więc `Pizza.objects.all()` uruchomi zapytanie w tabeli Toppings dla każdego elementu w Pizza QuerySet.

Czyli mamy do czynienia z problemem n+1 queries.

Aby uniknąć niepotrzebnych zapytań(n+1 query problem) użyjemy prefetch_related() ponieważ nie jest to relacja wiele do wielu.
```python
Pizza.objects.prefetch_related('toppings')
```

https://docs.djangoproject.com/en/4.2/ref/models/querysets/#prefetch-related
