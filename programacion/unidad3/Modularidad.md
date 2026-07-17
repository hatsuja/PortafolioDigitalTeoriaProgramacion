# Programación Modular

## 1. Modularizacion

La programación modular que permite dividir un programa complejo en unidades lógicas independientes llamadas **módulos** o **funciones**.

### Beneficios Principales
*   **Reutilización:** El código puede usarse en diferentes partes del proyecto sin duplicarse.
*   **Mantenimiento:** Es más sencillo localizar y corregir errores en un módulo específico.
*   **Legibilidad:** El programa principal se vuelve más corto y fácil de entender.


## 2. Funciones

Una función es un bloque de código diseñado para realizar una tarea específica, generalmente| una función puede recibir datos de entrada (parámetros) y retornar un resultado.

### Estructura Básica
* Retornar valor
```c
tipoRetorno nombreFuncion(tipoParametro parametro) {
    // Cuerpo de la función
    return valor;
}
```
* No retornar valor
```c
void nombreFuncion(tipoParametro parametro) {
    // Cuerpo de la función
}
```
## 3. Envío de Parámetros
El mecanismo de envío de parámetros determina cómo interactúa la función con los datos originales proporcionados.

### Envío por valor
La función recibe una copia del valor de la variable y cualquier modificación realizada dentro de la función no afecta a la variable original.

```c
#include <stdio.h>

void duplicarPorValor(int n) {
    printf(" Valor recibido: %d\n", n);
    n = n * 2;
    printf("Valor modificado: %d\n", n);
}

int main() {
    int numero = 10;
    
    printf("--- Pase por Valor ---\n");
    printf("Valor original: %d\n", numero);
    
    duplicarPorValor(numero);

    //Despues de la funcion

    printf("Valor final: %d\n", numero);
    printf("El valor original permanece intacto.\n");
    
    return 0;
}
```

### Envío por referencia
La función recibe la dirección de memoria (referencia) de la variable original y cualquier cambio realizado dentro de la función altera directamente a la variable original.

```c

#include <stdio.h>

void duplicarPorReferencia(int *n) {
    printf("Valor recibido: %d\n", *n);
    *n = *n * 2; // Modificamos el contenido de la direccion
    printf("Valor modificado: %d\n", *n);
}

int main() {
    int numero = 10;
    
    printf("--- Pase por Referencia ---\n");
    printf("Valor original: %d\n", numero);
    
    // Enviamos la direccion de memoria usando &
    duplicarPorReferencia(&numero);

    //Despues de la funcion
    
    printf("Valor final: %d\n", numero);
    printf("El valor original fue modificado.\n");
    
    return 0;
}

```

