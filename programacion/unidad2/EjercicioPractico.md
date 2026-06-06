
# <div align="center">Ejercicio Práctico: Simulador de Caja Registradora con Límite de Presupuesto</div>

---

## 3.1 Planteamiento del Problema

<p align="justify">
Un usuario desea realizar las compras del día en un supermercado local, pero cuenta con un presupuesto limitado (por ejemplo, $30.00). Para evitar quedarse sin fondos al momento de llegar a la caja general, se requiere el diseño de un programa informático en lenguaje C que simule una caja registradora portátil de control personal.
</p>

<p align="justify">
El algoritmo debe iniciar solicitando de forma obligatoria el ingreso del presupuesto total disponible. Posteriormente, mediante un ciclo iterativo, el usuario irá registrando secuencialmente el precio de cada producto que introduce en su carrito de compras.
</p>

**Reglas de negocio y restricciones basadas en condiciones:**
* El presupuesto ingresado al principio por el usuario debe ser un valor real estrictamente mayor a cero.
* El precio de cada artículo individual no puede ser una cantidad negativa. Si se detecta un valor erróneo, el programa debe obligar a reingresar el precio de forma persistente sin afectar el acumulador actual.
* Antes de sumar formalmente el costo de un nuevo producto al carrito, el sistema debe evaluar mediante una estructura condicional si dicha adición provocará que el gasto total acumulado exceda el presupuesto disponible. 
* Si el precio del producto hace que se supere el dinero disponible, el sistema debe denegar el ingreso del artículo, emitir una alerta textual de **"Presupuesto Excedido"** e interrumpir inmediatamente la ejecución del bucle.
* El proceso de compra repetitivo puede terminar de forma normal si el usuario digita un precio equivalente a `0`, lo cual indica que ha finalizado voluntariamente su selección de productos antes de agotar su dinero.

<p align="justify">
Al concluir la ejecución del ciclo (ya sea por alcanzar el límite de dinero o por decisión del comprador), el programa debe imprimir en pantalla un informe detallado con el total gastado y el saldo sobrante exacto que le queda en su billetera.
</p>

---

## 3.2 Análisis del Problema

* **Datos de Entrada:**
  * `float presupuesto`: Dinero total inicial con el que cuenta el usuario para comprar y debe ser( $> 0$).
   * `float precio_producto`: Costo individual de cada artículo que se desea agregar y debe ser( $\ge 0$).

* **Procesos Lógicos y Matemáticos:**
  * **Validación:** Uso de bucle (`do-while`) para controlar que el presupuesto inicial no sea cero ni negativo.
  * **Control de Iteración:** Uso de un bucle `while` controlado  por la condición implícita de que el gasto actual se mantenga por debajo del límite.
  * **Evaluación de Restricción Condicional (Estructura Selectiva):**
    * Si `(gasto_acumulado + precio_producto) > presupuesto` $\rightarrow$ El sistema activa la alerta, rechaza el producto y rompe el bucle utilizando la instrucción `break`.
    * Sino $\rightarrow$ El sistema acepta el artículo y actualiza las cuentas: `gasto_acumulado = gasto_acumulado + precio_producto`.
  * **Cálculo :** `saldo_restante = presupuesto - gasto_acumulado`.

* **Datos de Salida:**
  * Mensajes informativos interactivos por cada producto aceptado.
  * Reporte final: Monto total usado en el supermercado y el dinero sobrante.

---

## 3.1 Codificación en Lenguaje C


```c
#include <stdio.h>
int main() {
    float presupuesto, precio_producto, saldo_restante = 0.0, gasto_acumulado = 0.0;//variables
    printf("=== SIMULADOR DE CAJA REGISTRADORA===\n");
    do {
        printf("Ingrese su presupuesto: ");
        scanf("%f", &presupuesto);
        if (presupuesto <= 0) {
            printf("El presupuesto debe ser un monto mayor a 0.\n");
        }
    } while (presupuesto <= 0);
    printf("Ingrese el precio de los productos de 1 en 1.\n");
    printf("Digite '0' para finalizar las compras.\n");
    while (gasto_acumulado < presupuesto) {
        do {
            printf("Ingrese el precio del producto ($): ");
            scanf("%f", &precio_producto);
            if (precio_producto < 0) {
                printf("El precio de un producto no puede ser negativo.\n");
            }
        } while (precio_producto < 0);//  evitar el ingreso de precios negativos
        if (precio_producto == 0) {
            printf("Proceso finalizado.\n");
            break; // si el usuario ingresa 0 finaliza el ciclo
        }  
        if ((gasto_acumulado + precio_producto) > presupuesto) {
            printf("PRESUPUESTO EXCEDIDO y El producto de $%.2f no se puede agregar.\n", precio_producto);
            break; // interrupcion forzada del bucle por falta de fondos     
        } else {
            gasto_acumulado += precio_producto; // Suma el valor al acumulador
            printf("Producto agregado. Gasto actual: $%.2f\n", gasto_acumulado); // El producto esta dentro del presupuesto
        }
    }
    saldo_restante = presupuesto - gasto_acumulado;     // Calculo del saldo
    printf("\n=================================================================\n");
    printf("                     RESUMEN DE FACTURACION                      \n");
    printf("=================================================================\n");
    printf(" -> Presupuesto inicial     : $ %10.2f\n", presupuesto);
    printf(" -> Total gastado en caja   : $ %10.2f\n", gasto_acumulado);
    printf(" -> Dinero sobrante         : $ %10.2f\n", saldo_restante);
    printf("=================================================================\n");
    return 0;
}
```

