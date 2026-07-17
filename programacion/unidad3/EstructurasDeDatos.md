
# Estructuras de Datos Estáticas

## 1. Arreglos

Los arreglos son estructuras de datos que almacenan una colección de elementos del mismo tipo de forma contigua en la memoria y se consideran "estáticas" porque su tamaño debe definirse al momento de la compilación y no cambia durante la ejecución.


## 2. Arreglo Unidimensional (Vectores)
Es una lista de elementos organizados en una sola fila. Se accede a ellos mediante un único índice.

```c
#include <stdio.h>

int main() {
    // Problema: Calcular el promedio de 5 notas de una materia
    float notas[5] = {8.5, 9.0, 7.5, 10.0, 8.0};
    float suma = 0;

    printf("--- Registro de Notas ---\n");
    
    // Recorremos el arreglo para sumar las notas
    for(int i = 0; i < 5; i++) {
        printf("Nota %d: %.1f\n", i + 1, notas[i]);
        suma += notas[i];
    }

    printf("-------------------------\n");
    printf("Promedio final: %.2f\n", suma / 5);

    return 0;
}

```

## 3. Arreglo Bidimensional (Matrices)
Se organiza en filas y columnas. Es útil para representar tablas o cuadrículas, donde se requieren dos índices para localizar un dato.

```c
#include <stdio.h>

int main() {
    int matriz[2][2] = {{1, 2}, {3, 4}};

    printf("\n--- Arreglo Bidimensional ---\n");
    for(int i = 0; i < 2; i++) {
        for(int j = 0; j < 2; j++) {
            printf("Elemento en [%d][%d]: %d\n", i, j, matriz[i][j]);
        }
    }
    return 0;
}
```

## 4. Arreglo Multidimensional
Son arreglos con más de dos dimensiones (ej. un cubo). Se utilizan para representar datos complejos como volúmenes o series temporales de datos.
```c
#include <stdio.h>

int main() {
    // Cubo de 2x2x2
    int cubo[2][2][2] = {{{1, 2}, {3, 4}}, {{5, 6}, {7, 8}}};

    printf("\n--- Arreglo Multidimensional ---\n");
    printf("Valor en posicion [1][0][1]: %d\n", cubo[1][0][1]); // Imprime 6
    return 0;
}
```
