Curso completo en [campbi.com](https://campbi.com)

---
## Primer programa
En este programa introducimos la función `#!python print()` para imprimir datos.
``` py
print("Hola, este es mi primer programa.")
print("Segunda línea.")
print("Tercer línea.")
print(".............")
```

Respuesta:
```
Hola, este es mi primer programa.
Segunda línea.
Tercer línea.
.............
```

---

## Variables
Las variables son una forma de almacenar datos de cualquier tipo.

### Declaración de variables

* Declaración de nuevas variables:
``` py
nombre_usuario = "Sebastian"
```
* Declaración de variables de tipo constante:
``` py
NOMBRE_EQUIPO = "mypc"
```
* Reasignación de variables:
``` py
edad_usuario = 12
edad_usuario = edad_usuario + 12 
```

### Reglas de nombramiento

* Nombramiento de variables:
    * Deben comenzar con una letra o un guion bajo ("-").
    * Pueden contener letras, números y guiones bajos.
    * Python distingue entre mayúsculas y minúsculas, es decir, nombre y Nombre son variables diferentes.

* Nombres significativos:
    * Nombres descriptivos que reflejen el propósito o contenido de la variable
    ``` py
        # Evitar
        x = 5

        # Bueno
        edad_usuario = 25 
    ```
* Evitar nombres de variables de una letra.
* Evitar palabras reservadas de Python como: `#!python if`, `#!python while`, `#!python for`, `#!python class`, etc.
* Evitar guiones bajos iniciales
    ``` py
        # Evitar
        _variable_privada = 42
    ```
---

## Tipos de datos
Son utilizados para representar los diferentes tipos de valores que un programa puede manipular.

* Enteros (`#!python int`): Representan números enteros sin decimales.
    ``` py
        edad = 25
        cuenta_regresiva = -45
    ```
* Flotantes (`#!python float`): Representan números decimales.
    ``` py
        pi = 3.14159
        altura = 1.90
    ```
* Cadenas de texto (`#!python str`): Representan secuencias de caracteres. Pueden contener letras, números y caracteres especiales.
    ``` py
        nombre = "Juan"
        mensaje = "Hola, ¿Cómo estás?"
    ```
* Booleanos (`#!python bool`): Representan valores de verdad: True o False.
    ``` py
        es_mayor_de_edad = True
        esta_lloviendo = False
    ```

* None (`#!python None`): Representa la ausencia de valor o la falta de un valor válido. 
    ``` py
        resultado = None
    ```

### Validar un tipo de dato
La función `#!python type()` nos permite validar a que tipo de dato corresponde un valor:
    ``` py
        edad_usuario = 34
        print(type(edad_usuario))
    ```
Respuesta:
    ```
         <class 'int'>
    ```

### Métodos y acciones
#### Strings:
* `#!python upper()`: Convierte un texto a máyuscula.
    ``` py
        nombre_usuario = "santiago"
        nombre_usuario = nombre_usuario.upper() # SANTIAGO
    ```
* `#!python lower()`: Convierte un texto a mínuscula.
    ``` py
        nombre_usuario = "SANTIAGO"
        nombre_usuario = nombre_usuario.lower() # santiago
    ```
* `#!python capitalize()`: Convierte en máyuscula la primer letra del texto.
    ``` py
        mensaje = "hola, bienvenido."
        mensaje = mensaje.capitalize() # Hola, bienvenido.
    ```
* `#!python title()`: Convierte en máyuscula la primer letra de cada palabra.
    ``` py
        usuario = "andres felipe"
        usuario = usuario.title() # Andres Felipe
    ```
* `#!python count()`: Cuenta la cantidad de apariciones de un caracter dentro de un texto.
    ``` py
        usuario = "andres felipe"
        usuario = usuario.count(e) # 3
    ```
* `#!python find()`: Regresa la posición inicial de una subcadena de texto dentro de un texto.
    ``` py
        usuario = "santiago wilches"
        usuario = usuario.find("wilches") # 9
    ```
* `#!python replace()`: Remplaza una subcadena de texto por otra.
    ``` py
        mensaje = "Hola, bienvenido."
        mensaje = mensaje.replace("Hola", "Chao") # Chao, bienvenido.
    ```
* `#!python strip()`: Elimina los espacios en blanco al inicio y al final de un texto.
    ``` py
        mensaje = "  Hola, bienvenido.  "
        mensaje = mensaje.strip() # Hola, bienvenido.
    ```
* `#!python strip()`: Elimina los espacios en blanco al inicio y al final de un texto.
    ``` py
        mensaje = "  Hola, bienvenido.  "
        mensaje = mensaje.strip() # Hola, bienvenido.
    ```
* `#!python startswith()`: Comprueba si una cadena de texto comienza con una subcadena específica.
    ``` py
        mensaje = "Hola, bienvenido."
        mensaje = mensaje.startswith("Hola") # True
    ```
* `#!python endswith()`: Comprueba si una cadena de texto termina con una subcadena específica.
    ``` py
        mensaje = "Hola, bienvenido."
        mensaje = mensaje.endswith("Hola") # False
    ```
* `#!python len()`: Regresa la longitud de un objeto.
    ``` py
        mensaje = "Hola"
        mensaje = len(mensaje) # Hola
    ```
* `#!python +`: Concatena cadenas de texto.
    ``` py
        nombre = "Andrew"
        apellido = "Smith
        nombre_completo = nombre + " " + apellido # Andrew Smith
    ```
* `#!python *`: Concatena el mismo texto n cantidad de veces.
    ``` py
        nombre = "Andrew"
        nombre = nombre * 4 # AndrewAndrewAndrewAndrew
    ```
#### Números:
* `#!python abs()`: Regresa el valor absoluto de un número.
    ``` py
        temperatura = -22
        temperatura = abs(temperatura) # 22
    ```
* `#!python round()`: Aproxima un número con decimales al número entero más cercano.
    ``` py
        temperatura = 22.3
        temperatura = round(temperatura) # 22
    ```

### Conversión de tipos de datos
* `#!python int()`: Convertir a entero.
    ``` py
        numero_string = "2223"
        type(int(2223)) # int
    ```
* `#!python str()`: Convertir a string.
    ``` py
        numero = 1234
        type(str(numero)) # str
    ```
