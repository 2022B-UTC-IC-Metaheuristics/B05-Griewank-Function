# Griewank-Function
![](https://www.sfu.ca/~ssurjano/griewank.png)


![](https://www.sfu.ca/~ssurjano/griewank2.png)
### Descripción:
*Dimensiones*: d

La función Griewank tiene muchos mínimos locales generalizados, que se distribuyen regularmente. La complejidad se muestra en los gráficos ampliados.

### Dominio de entrada:
La función se evalúa normalmente en el hipercubo xi ∈ [-600, 600], para todo i = 1, ..., d.

### Minimo Global:
![](https://www.sfu.ca/~ssurjano/griewank3.png)

### Codigo:

```Python
def griewank_function(vector):
    tam = len(vector)
    sum = 0
    prod = 1

    for i in range(tam):
        x = vector[i]
        sum = sum + (x**2)/4000
        prod = prod * math.cos(x/math.sqrt(i+1))
        
    return sum - prod + 1
```

# Contribuciones 
Uribe Matus Miguel Angel

Lopez Ituarte Austin
