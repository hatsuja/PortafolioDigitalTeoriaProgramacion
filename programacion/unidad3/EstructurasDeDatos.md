<div align="center">
    
# Estructuras de datos estáticas

</div>

## 1. Arreglos

Los arreglos son estructuras de datos que almacenan una colección de elementos del mismo tipo en la memoria y se consideran "estáticas" porque su tamaño debe definirse al momento de la compilación y no cambia durante la ejecución.


## 2. Arreglo Unidimensional (Vectores)
Es una lista de elementos organizados en una sola fila. Se accede a ellos mediante un único índice.

<div align="center">
    
<img width="385" height="152" alt="image" src="https://github.com/user-attachments/assets/a34ed611-fecf-4b02-a275-fcf2f8c8619c" />

</div>

### Ejemplo


```c
#include <stdio.h>

int main() {
    // Problema: Calcular el promedio de 5 notas de una materia
    float notas[5] = {8.5, 9.0, 7.5, 10.0, 8.0};
    float suma = 0;

    printf("--- Registro de Notas ---\n");
    

    for(int i = 0; i < 5; i++) {
        printf("Nota %d: %.1f\n", i + 1, notas[i]);
        suma += notas[i];
    }

    printf("-------------------------\n");
    printf("Promedio final: %.2f\n", suma / 5);

    return 0;
}

```
### Prueba de Escritorio

<img width="247" height="182" alt="image" src="https://github.com/user-attachments/assets/963a1aa1-881c-4765-964c-0139107c5eea" />



## 3. Arreglo Bidimensional (Matrices)
Se organiza en filas y columnas. Es útil para representar tablas o cuadrículas, donde se requieren dos índices para localizar un dato.

<img width="1000" height="314" alt="GIffor2D3D11" src="https://github.com/user-attachments/assets/9fa736de-5ade-4870-9f6a-b85be3e4cfc2" />


### Ejemplo


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

### Prueba de Escritorio

<img width="526" height="85" alt="image" src="https://github.com/user-attachments/assets/e92b3ea9-d1d5-40e6-bdc4-05b762e31f60" />


## 4. Arreglo Multidimensional

Son arreglos con más de dos dimensiones (ej. un cubo). Se utilizan para representar datos complejos como volúmenes o series temporales de datos.


<img width="1000" height="470" alt="GIffor2D3Dcube" src="https://github.com/user-attachments/assets/e9f97cdd-6150-40e7-86f4-082b58a31ebd" />


### Ejemplo

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
### Prueba de Escritorio

<img width="432" height="241" alt="image" src="https://github.com/user-attachments/assets/202df8c8-e5b7-4acf-b5f0-615f0f232832" />


<p align="center">
  <a href="https://github.com/hatsuja/PortafolioDigitalTeoriaProgramacion/blob/main/index.md">
    <b>📂 Ir al Índice Principal 📂</b>
  </a>
</p>

