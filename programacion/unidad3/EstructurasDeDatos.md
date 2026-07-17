<div align="center">
    
# Estructuras de Datos Estáticas

</div>

## 1. Arreglos

Los arreglos son estructuras de datos que almacenan una colección de elementos del mismo tipo en la memoria y se consideran "estáticas" porque su tamaño debe definirse al momento de la compilación y no cambia durante la ejecución.


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
    // Problema: Registrar y promediar la temperatura de 3 ciudades en 4 semanas
    float temps[3][4] = {
        {22.5, 23.0, 21.5, 22.0}, // Ciudad A
        {18.0, 19.5, 17.5, 18.5}, // Ciudad B
        {25.0, 26.0, 24.5, 25.5}  // Ciudad C
    };
    
    char* ciudades[] = {"Ciudad A", "Ciudad B", "Ciudad C"};
    float suma;

    printf("--- Reporte de Temperaturas Promedio ---\n");

    for(int i = 0; i < 3; i++) {
        suma = 0;
        printf("%s: ", ciudades[i]);
        
        for(int j = 0; j < 4; j++) {
            printf("%.1f  ", temps[i][j]);
            suma += temps[i][j];
        }
        
        printf("| Promedio: %.2f\n", suma / 4);
    }

    return 0;
}

```

## 4. Arreglo Multidimensional
Son arreglos con más de dos dimensiones (ej. un cubo). Se utilizan para representar datos complejos como volúmenes o series temporales de datos.
```c
#include <stdio.h>

int main() {
    // Problema: Inventario de camisas
    // Dimensiones: [Sucursal][Talla][Color]
    
    int inventario[2][2][2] = {
        { // Sucursal Norte
            {10, 15}, // Talla M: 10 blancos, 15 negros
            {8, 12}   // Talla L: 8 blancos, 12 negros
        },
        { // Sucursal Sur
            {5, 7},   // Talla M: 5 blancos, 7 negros
            {20, 25}  // Talla L: 20 blancos, 25 negros
        }
    };

    printf("--- Control de Inventario Tridimensional ---\n");
    
    // Recorrido del cubo de datos
    for(int s = 0; s < 2; s++) {
        printf("Sucursal %d:\n", s);
        for(int t = 0; t < 2; t++) {
            for(int c = 0; c < 2; c++) {
                printf("  Talla %d, Color %d: %d unidades\n", t, c, inventario[s][t][c]);
            }
        }
    }

    return 0;
}
```
