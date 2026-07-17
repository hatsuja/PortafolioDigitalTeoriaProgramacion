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
```cpp
tipoRetorno nombreFuncion(tipoParametro parametro) {
    // Cuerpo de la función
    return valor;
}

3. Envío de Parámetros
El mecanismo de envío de parámetros determina cómo interactúa la función con los datos originales proporcionados por el llamador.

3.1. Pase por Valor
En este modo, la función recibe una copia del valor de la variable.

Comportamiento: Cualquier modificación realizada dentro de la función no afecta a la variable original.

Uso ideal: Cuando solo necesitamos leer el dato pero proteger la integridad de la variable original.
