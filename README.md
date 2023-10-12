# Reto_7_odioelpunto6
# Punto 1
1. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
![](https://i.ibb.co/J7MqkQ8/PUNTO-1-1.png)
```
x = 1
y = 1
while x <= 100:
   print(x, y, sep = ", ")
   x = x +1
   y = x ** 2
```
# Punto 2
2.  Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
![](https://i.ibb.co/TcTY9M4/Punto-2.png)

```
x = 1
y = 1
while x <= 999:
  x += 1
  if x % 2 == 0:
    continue
  print(x)
while y <= 1000:
  y += 1
  if y % 2 != 0:
    continue
  print(y)
```
# Punto 3
3.  Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado
```
n= int(input("Ingrese un número natural mayor o igual a dos: "))
while n>=2:
    n -=1
    if n%2!=0:
        continue
    print(n)
```
# Punto 4
4. En 2022 el país A tendrá una población de 25 millones de habitantes y el país B de 18.9 millones. Las tasas de crecimiento anual de la población serán de 2% y 3% respectivamente. Desarrollar un algoritmo para informar en que año la población del país B superará a
la de A.
```
a : int = 25000000
b : int = 18000000
c : int = 2022
while(a > b):
  a *= (1+ 0.02) #acá se factorizó, el original quedaría a = a por (a más a por 0.002)
  b *= (1+ 0.03) #La misma situación acá
  c += 1
print(a, b, c)
print(f"En el año {c} la ciudad b supera a la ciudad a con un total de {b} habitantes" )
```
# Punto 5
5. Imprimir el factorial de un número natural n dado.
```
n : int
n = int(input("Ingrese un valor:"))
y : int = 1
z : int = 1
while y <= n:
    z = z * y
    y = y + 1
print(f"El factorial del número {n} es {z}") 
```
# Punto 6
6. Implementar un algoritmo que permita adivinar un número dado de 1 a 100, preguntando en cada caso si el número es mayor, menor o igual.
```
print("A que logro adivinar su número ")
x : int = 100
y : int = 0
i2 : int = 0
z = True

while z:
    i = (y + x)//2
    i2 = i2 + 1
    a1 = input(f"su número es {i} si(c), mayor(a), menor(b) ?")
    if a1 == "b":
      x = i + 1
    elif a1 == "a":
      y = i - 1
    elif a1 == "c":
      print(f"Su número es {i}")
      break
    else:
       print("respuesta no válida recuerde digitar las letras en minuscula")
```
# Punto 7
7. Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.
```
y = int(input("Ingrese un número entre 2 y 50:"))

if 2 <= y <= 50:
    x = 2
    while x <= 50:
        if x % y == 0:
            print(x)
        x += 1
else:
    print("El número tiene que estar entre 2 y 50")
```
# punto 8
8. Implementar el algoritmo que muestre los números primos del 1 al 100. **Nota:** use funciones
```
n = 1

while n <= 100:
    if n > 1:
        p = True
        d = 2
        while d * d <= n:
            if n % d == 0:
                p = False
                break
            d += 1
        if p:
            print(n)
    n += 1
```
