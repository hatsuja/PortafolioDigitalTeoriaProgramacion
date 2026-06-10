
# <div align="center">Ejercicio Práctico: Simulador de Caja Registradora con Límite de Presupuesto</div>

---

## 3.1 Planteamiento del Problema

<p align="justify">
Un usuario desea realizar las compras del día en un supermercado local, pero cuenta con un presupuesto limitado (por ejemplo, $30.00). Para evitar quedarse sin fondos al momento de llegar a la caja general, se requiere el diseño de un programa informático en lenguaje C que simule una caja registradora portátil de control personal.
</p>

<p align="justify">
El algoritmo debe iniciar solicitando de forma obligatoria el ingreso del presupuesto total disponible. Posteriormente, mediante un ciclo iterativo, el usuario irá registrando secuencialmente el precio de cada producto que introduce en su carrito de compras.
</p>

**Reglas y restricciones:**
* El presupuesto ingresado al principio por el usuario debe ser un valor real mayor a cero.
* El precio de cada artículo individual no puede ser una cantidad negativa. Si se detecta un valor erróneo, el programa debe obligar a reingresar el precio de forma persistente sin afectar el acumulador actual.
* Antes de sumar formalmente el costo de un nuevo producto al carrito, el sistema debe evaluar mediante una estructura condicional si dicha adición provocará que el gasto total acumulado exceda el presupuesto disponible. 
* Si el precio del producto hace que se supere el dinero disponible, se debe denegar el ingreso del artículo, emitir una alerta e interrumpir inmediatamente la ejecución del bucle.
* El proceso de compra repetitivo puede terminar de forma normal si el usuario digita un precio equivalente a `0`, lo cual indica que ha finalizado voluntariamente su selección de productos antes de agotar su dinero.

<p align="justify">
Al concluir la ejecución del ciclo (ya sea por alcanzar el límite de dinero o por decisión del comprador), el programa debe imprimir en pantalla un informe detallado con el total gastado y el saldo sobrante exacto que le queda en su billetera.
</p>


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
  * Dinero total usado en el supermercado y el dinero sobrante.

## 3.3 Diagrama de flujo
<p align="center">
<img width="489" height="1661" alt="protafolio drawio" src="https://github.com/user-attachments/assets/797f0fb1-4a9b-4fa7-a06e-a5140a3213b6" />
</p>

## 3.4 Codificación en Lenguaje C


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
## 3.5 Prueba de escritorio
* ### Resultado de la Terminal

<p align="center">
<img width="637" height="442" alt="image" src="https://github.com/user-attachments/assets/f7847683-e60b-46f2-a933-f86fed383114" />
</p>

* ### Calculos

| Paso / Bucle | presupuesto | precio_producto | gasto_acumulado | saldo_restante | Condición: ¿Excede presupuesto?<br>`(gasto_acumulado + precio_producto) > presupuesto` | Acción del programa / Salida en pantalla |
| :--- | :---: | :---: | :---: | :---: | :--- | :--- |
| **0. Inicio** | ? | ? | 0.00 | 0.00 | No aplica | Muestra: `"=== SIMULADOR DE CAJA REGISTRADORA==="` |
| **1. Entrada** | 50.00 | ? | 0.00 | 0.00 | No aplica | El usuario ingresa 50. Muestra instrucciones. |
| **2. Iteración 1** | 50.00 | 2.00 | 2.00 | 0.00 | `(0.00 + 2.00) > 50.00` ➔ **FALSO** | Suma al gasto. Muestra: `"Producto agregado. Gasto actual: $2.00"` |
| **3. Iteración 2** | 50.00 | 40.00 | 42.00 | 0.00 | `(2.00 + 40.00) > 50.00` ➔ **FALSO** | Suma al gasto. Muestra: `"Producto agregado. Gasto actual: $42.00"` |
| **4. Iteración 3** | 50.00 | 20.00 | 42.00 | 0.00 | `(42.00 + 20.00) > 50.00` ➔ **VERDADERO** (62.00 > 50.00) | No suma. Muestra: `"PRESUPUESTO EXCEDIDO..."` ➔ Se ejecuta el `break` (sale del bucle). |
| **5. Cálculo Final** | 50.00 | 20.00 | 42.00 | 8.00 | No aplica | Calcula: `saldo_restante = 50.00 - 42.00` |
| **6. Fin** | 50.00 | 20.00 | 42.00 | 8.00 | No aplica | Imprime el bloque del **RESUMEN DE FACTURACIÓN**. |



<p align="center">
  <a href="https://github.com/hatsuja/PortafolioDigitalTeoriaProgramacion/blob/main/index.md">
    <b>📂 Ir al Índice Principal 📂</b>
  </a>
</p>

