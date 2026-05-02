# <p align="center">Programacion en C</p>

## El Lenguaje C

 Es un lenguaje de nivel medio que combina la potencia del lenguaje ensamblador con la facilidad de los lenguajes de alto nivel y fue desarrollado por Dennis Ritchie en los laboratorios Bell en 1972.

>Es ideal para crear sistemas operativos, compiladores y software que requiera alta velocidad siendo un lenguaje compilado, lo que significa que el código fuente se traduce totalmente a lenguaje máquina antes de ejecutarse

---
## Estructura de un Programa en C

* ### Archivo

El código se guarda en archivos con extensión `.c`

* ### Bibliotecas

las bibliotecas las cuales se usan para incluir funciones externas

>#include <stdio.h>

>#include <stdlib.h>

>#include <string.h>

>#include <math.h>

>#include <time.h>

* ### Función principal

La función principal que es el (main) el cual es el punto de inicio de cualquier programa en C y odo el código que se ejecuta va dentro de llaves { }

* ### Ejemplo

```
#include<stdio.h>
int main(){
   //proceso
return 0;
} 
```

* ### Compilacion y ejecución

Por lo general para complicar se usa 
``` 
gcc .\hola_mundo.c -o hola_mundo
```
>El compilador traduce directamente el código a lenguaje máquina

Y para ejecutar 
``` 
.\hola_mundo.exe
```
>El archivo corre directamente en el Sistema Operativo

---

## Tipo de datos 

<div align="center">

| Tipo de Dato | ¿Qué guarda? | Ejemplo de Declaración |
| :---: | :--- | :--- |
| `int` | Números enteros (sin decimales), positivos o negativos | `int edad = 20;` |
| `float` | Números con decimales sencillos | `float precio = 10.50;` |
| `double` | Números con decimales más largos o precisos | `double pi = 3.14159265;` |
| `char` | Una sola letra, número o símbolo | `char letra = 'A';` |
| `char[]` | un grupo de caracteres | `char nombre[] = "Hatsu";` |
| `const` | Un valor que **no cambia** en todo el programa | `const int IVA = 16;` |
| `#define` | Define un valor fijo al inicio del código | `#define TASA 0.15` |

</div>

>Variables: Son como "cajas" donde guardas información que puede cambiar mientras el programa corre

>Constantes: Se usan para valores que deben permanecer fijos, como el valor de PI o un porcentaje de impuesto

---
## Operadores de Asignación Compuesta

<div align="center">

###
Estos operadores permiten realizar una operación aritmética y asignar el resultado a la misma variable de forma abreviada:

| Operador | Ejemplo | Equivalencia | Descripción |
| :--- | :---: | :---: | :--- |
| **Básico** | `c = a + b;` | N/A | Asigna a `c` el resultado de la suma |
| **Suma** | `a += b;` | `a = a + b;` | Suma `b` al valor actual de `a` |
| **Resta** | `a -= b;` | `a = a - b;` | Resta `b` al valor actual de `a` |
| **Multiplicación** | `a *= b;` | `a = a * b;` | Multiplica `a` por `b` |
| **División** | `a /= b;` | `a = a / b;` | Divide `a` entre `b`|
| **Módulo** | `a %= b;` | `a = a % b;` | Asigna el residuo de la división |

</div>


