# reto-4
El desarrollo de este reto se encuentra en el siguiente cuaderno de Google Colab: https://colab.research.google.com/drive/1h4CIulbpTz9TlAhSqaObxmu1fUip5PMy?hl=es#scrollTo=W7xvXfxTQB5e

#Punto 1
```python
a : int
a = int(input('Escriba un número entero en código ASCII:'))
match a:

  case '97':
    print('El código ASCII 97 corresponde a la vocal minúscula a')
  case '101':
    print('El código ASCII 101 corresponde a la vocal minúscula e')
  case '105':
    print('El código ASCII 105 corresponde a la vocal minúscula i')
  case '111':
    print('El código ASCII 111 corresponde a la vocal minúscula o')
  case '117':
    print('El código ASCII 117 corresponde a la vocal minúscula u')
  case _:
    print('El código ASCII ingresado no pertenece a ninguna vocal minúscula')
```

#Punto 2

```pyhton
lang = input('Escriba solo un número, letra o símbolo:')
lang1 = ord(lang)
if lang1%2 == 0:
  print('El código ASCII de ' +str(lang)+ ' es ' +str(lang1)+ ', y por lo tanto, es un número par')
else:
  print('El código ASCII de ' +str(lang)+ ' es ' +str(lang1)+ ', y por lo tanto, es un número impar')
```

#Punto 3

```python
lang = input('Escriba un único carácter:')
if lang.isdigit():
  print('El carácter ' +str(lang)+ ' es un dígito')
else:
  print('El carácter ' +str(lang)+ ' no es un dígito')
```

#Punto 4

```python
n : float
n = float(input('Escriba un número real:'))
if n < 0:
  print('El número ' +str(n)+ ' es un número negativo')
elif n > 0:
  print('El número ' +str(n)+ ' es un número positivo')
elif n == 0:
  print('El número ' +str(n)+ ' es el neutro para la suma')
```

#Punto 5

```python
a : float ##Esta es la coordenada en x del centro del círculo
b : float ##Esta es la coordenada en y del centro del círculo
c : float ##Este es el radio del círculo
d : float ## Esta es la coordenada en x de un punto de R2
e : float ##Esta es la coordenada en y de un punto de R2
f : float ##Esta es la ecuación formada por los puntos ingresados
a = float(input('Escriba la coordenada en X del centro del círculo:'))
b = float(input('Escriba la coordenada en Y del centro del círculo:'))
c = float(input('Escriba el radio del círculo:'))
d = float(input('Escriba la coordenada en X de algún punto de R2:'))
e = float(input('Escriba la coordenada en Y de algún punto de R2:'))
f = (d-a)**2+(e-b)**2
if f < c**2:
  print('El punto ' '(' +str(d)+ ' , ' +str(e)+ ') pertenece al interior del círculo')
elif f > c**2:
  print('El punto ' '(' +str(d)+ ' , ' +str(e)+ ') no pertenece al interior del círculo')
elif f == c**2:
  print('El punto ' '(' +str(d)+ ' , ' +str(e)+ ') pertenece a la circunferencia del círculo')
```

#Punto 6

```python
a : float
b : float
c : float
a = float(input('Escriba la primera longitud:'))
b = float(input('Escriba la segunda longitud:'))
c = float(input('Escriba la tercera longitud:'))
if a+b>c:
  print('Es posible generar un triángulo usando las longitudes ' +str(a)+ ', ' +str(b)+ ' y ' +str(c))
elif a+c>b:
  print('Es posible generar un triángulo usando las longitudes ' +str(a)+ ', ' +str(b)+ ' y ' +str(c))
elif c+b>a:
  print('Es posible generar un triángulo usando las longitudes ' +str(a)+ ', ' +str(b)+ ' y ' +str(c))
else:
  print('No es posible generar un triángulo usando las longitudes ' +str(a)+ ', ' +str(b)+ ' y ' +str(c))
```
