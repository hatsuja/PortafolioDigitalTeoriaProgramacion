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
```c
tipoRetorno nombreFuncion(tipoParametro parametro) {
    // Cuerpo de la función
    return valor;
}
```

## 3. Envío de Parámetros
El mecanismo de envío de parámetros determina cómo interactúa la función con los datos originales proporcionados por el llamador.

### Pase por Valor
La función recibe una copia del valor de la variable y cualquier modificación realizada dentro de la función no afecta a la variable original.

```c
void sumarDiez(int numero) {
    numero = numero + 10; // Solo cambia la copia
}

int main() {
    int x = 5;
    sumarDiez(x);
    // x sigue valiendo 5
}
}
```

### Pase por Referencia
La función recibe la dirección de memoria (referencia) de la variable original y cualquier cambio realizado dentro de la función altera directamente a la variable origina

```c
void sumarDiez(int &numero) {
    numero = numero + 10; // Cambia el original
}

int main() {
    int x = 5;
    sumarDiez(x);
    // x ahora vale 15
}
```

