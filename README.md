# Reto_4

## 1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.

codigo:
```
numero = int(input("Ingrese un número entero: "))

if numero == 97 or numero == 101 or numero == 105 or numero == 111 or numero == 117:
    print(f"El número {numero} corresponde al código ASCII de una vocal minúscula.")
else:
    print(f"El número {numero} no corresponde al código ASCII de una vocal minúscula.")
```

## 2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.

codigo:
```
adena = input("Ingrese una cadena de longitud 1: ")

if len(cadena) == 1:
    codigo_ascii = ord(cadena)
    
    if codigo_ascii % 2 == 0:
        print(f"El código ASCII de la primera letra '{cadena}' es par.")
    else:
        print(f"El código ASCII de la primera letra '{cadena}' no es par.")
else:
    print("La cadena debe tener longitud 1.")
```

## 3. Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.

codigo:
```
caracter = input("Ingrese un carácter: ")

if caracter >= '0' and caracter <= '9':
    print(f"El carácter '{caracter}' es un dígito.")
else:
    print(f"El carácter '{caracter}' no es un dígito.")
```

## 4. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

*   Positivo: "El número x es positivo"
*   Negativo: "El número x es negativo"
*   Cero (0): "El número x es el neutro para la suma"

codigo:
```
x = float(input("Ingrese un número real: "))

if x > 0:
    print(f"El número {x} es positivo.")
elif x < 0:
    print(f"El número {x} es negativo.")
else:
    print(f"El número {x} es el neutro para la suma.")
```

## 5. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.

codigo:
```
centro_x = float(input("Ingrese la coordenada x del centro del círculo: "))
centro_y = float(input("Ingrese la coordenada y del centro del círculo: "))
radio = float(input("Ingrese el radio del círculo: "))
punto_x = float(input("Ingrese la coordenada x del punto: "))
punto_y = float(input("Ingrese la coordenada y del punto: "))

distancia = ((punto_x - centro_x) ** 2 + (punto_y - centro_y) ** 2) ** 0.5

if distancia < radio:
    print("El punto está dentro del círculo.")
else:
    print("El punto no está dentro del círculo.")
```

## 6. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.

codigo:
```
lado1 = float(input("Ingrese la longitud del primer lado: "))
lado2 = float(input("Ingrese la longitud del segundo lado: "))
lado3 = float(input("Ingrese la longitud del tercer lado: "))

if lado1 + lado2 > lado3 and lado1 + lado3 > lado2 and lado2 + lado3 > lado1:
    print("Se puede construir un triángulo con estas longitudes.")
else:
    print("No se puede construir un triángulo con estas longitudes.")
```
