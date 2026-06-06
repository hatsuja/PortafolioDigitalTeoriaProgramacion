
<br>
---

# <div align="center">2. Estructuras Repetitivas</div>
---

<br>

## 2.1 ¿Qué son las Estructuras Repetitivas?

<p align="justify">
Las estructuras repetitivas (también conocidas como bucles, ciclos o estructuras de iteración) son instrucciones de control que permiten ejecutar un bloque específico de código múltiples veces. La repetición se mantiene activa de forma cíclica mientras una condición lógica determinada (expresión booleana) se evalúe como verdadera, o hasta que se alcance un número predeterminado de iteraciones.
</p>

<p align="justify">
En el desarrollo de software, estas estructuras son indispensables porque automatizan tareas rutinarias o masivas (como procesar las notas de un grupo de estudiantes), optimizan significativamente la longitud del código fuente y evitan la duplicación innecesaria de instrucciones lineales dentro del programa.
</p>

---

## 2.2 Tipos de Estructuras Repetitivas

<p align="justify">
Dependiendo del momento en que se evalúe la condición de control y de si se conoce o no de antemano el número exacto de iteraciones, los bucles se clasifican técnicamente en las siguientes categorías:
</p>

### A. Estructura Mientras (`while`)
<p align="justify">
Es una estructura de pre-prueba. Esto significa que evalúa la condición lógica <b>antes</b> de permitir el ingreso al bloque de código. Si la condición es verdadera, ejecuta las instrucciones en su interior y vuelve a evaluar; si es falsa desde la primera comprobación, el bucle no se ejecuta ni una sola vez. Es ideal cuando el número de repeticiones depende de factores externos variables durante la ejecución.
</p>

### B. Estructura Hacer .. Mientras / Repetir .. Hasta (`do while`)
<p align="justify">
Es una estructura de post-prueba. A diferencia del bucle anterior, la condición de control se evalúa <b>al final</b> de la iteración. Esto garantiza con total certeza que el bloque de instrucciones interno se ejecutará <b>al menos una vez</b>, sin importar si la condición es falsa desde el principio. Es la estructura estándar utilizada para la validación de datos de entrada (por ejemplo, asegurar que una nota esté obligatoriamente en el rango de 0 a 10).
</p>

### C. Estructura Para (`for`)
<p align="justify">
Es una estructura de control especializada en la iteración contada. Se utiliza cuando el programador conoce con exactitud el número de veces que se debe repetir el ciclo antes de que este inicie. Integra en una sola línea tres componentes esenciales: la inicialización de una variable contador, la condición de parada o límite, y la expresión de incremento o decremento que actualiza el contador tras cada iteración.
</p>

### D. Anidamiento de estructuras repetitivas
<p align="justify">
El anidamiento ocurre cuando se coloca una estructura repetitiva (bucle interno) dentro del cuerpo de instrucciones de otra estructura repetitiva (bucle externo). Por cada iteración única que realiza el ciclo externo, el ciclo interno ejecuta su secuencia de repeticiones completa de principio a fin. Esta técnica es fundamental para trabajar con estructuras de datos complejas multidimensionales, como matrices, tablas de coordenadas o para procesar múltiples componentes evaluativos por cada estudiante.
</p>

---

## 2.3 Pseudocódigo de cada Tipo de Estructura

<p align="justify">
A continuación, se detalla la sintaxis lógica y la organización estructural en formato de pseudocódigo estándar para cada bucle analizado:
</p>

### Pseudocódigo: Estructura Mientras (`while`)
```text
Mientras (condicion_logica) Hacer
    // Bloque de instrucciones a repetir
    // (Debe incluir la modificación de la variable de control)
FinMientras
