

# <div align="center">Estructuras Condicionales</div>



## 1.1 ¿Qué son las Estructuras Condicionales?

<p align="justify">
Las estructuras condicionales (también conocidas como estructuras de bifurcación o selectivas) son instrucciones de control que permiten alterar el flujo lineal y secuencial de la ejecución de un programa siendo su propósito principal es evaluar una condición lógica o una expresión booleana que puede resultar únicamente en verdadero o falso y, en función de dicho resultado, desviar el camino del flujo para ejecutar un bloque específico de código.
</p>

<p align="justify">
En el ámbito del desarrollo de software, estas estructuras dotan a los algoritmos de la capacidad de tomar decisiones dinámicas en tiempo real en base a los datos de entrada proporcionados por el usuario o por el entorno físico de ejecución, evitando que el programa actúe siempre de la misma forma rígida.
</p>

---

## 1.2 Tipos de Condicionales

<p align="justify">
Dependiendo de la complejidad de la decisión y de la cantidad de caminos opcionales que se presenten en el problema, las estructuras selectivas se clasifican técnicamente en tres categorías:
</p>

### A. Estructuras condicionales simples (`if`)
<p align="justify">
Es la variante básica de selección. Evalúa una única condición lógica; si esta se cumple (es verdadera), el programa ingresa y procesa las instrucciones delimitadas en su interior. En caso de que la condición no se cumpla (es falsa), el bloque interno es completamente ignorado y el compilador continúa con la ejecución lineal de la siguiente línea de código externa.
</p>

### B. Estructuras condicionales dobles (`if else`)
<p align="justify">
Permiten dividir el flujo del algoritmo en dos rutas alternativas que son mutuamente excluyentes entre sí. Al evaluarse la expresión de control, si el resultado es verdadero, se procesa obligatoriamente el bloque del <code>if</code>; de lo contrario, si la expresión resulta ser falsa, el flujo se desvía sin excepción para ejecutar el bloque secundario definido bajo la palabra reservada <code>else</code> (sino).
</p>

### C. Estructuras condicionales múltiples (`if else if`, `case` / `switch`)
<p align="justify">
Se implementan cuando la naturaleza del problema exige evaluar más de dos caminos posibles dependientes de diversas combinaciones lógicas o del estado numérico de una variable particular.
</p>

* **Estructura `if else if` (Anidada):** Se encarga de evaluar de forma ordenada y secuencial una serie de condiciones distintas. En el preciso instante en que una de las expresiones lógicas resulta verdadera, se ejecuta su respectivo bloque interno y el programa sale automáticamente de toda la estructura de control, omitiendo las validaciones restantes.
* **Estructura `case` o `switch` (Selección Múltiple):** Es una alternativa optimizada para evaluar el valor exacto de una única variable cuantitativa (generalmente de tipo entero o carácter). Compara dicho valor de forma directa contra una serie de casos preestablecidos (<code>case</code>). Si encuentra una coincidencia exacta, procesa ese bloque; opcionalmente incluye una sección por defecto (<code>default</code> o de otro modo) para manejar situaciones no previstas.

---

## 1.3 Pseudocódigo de cada Tipo de Estructura

<p align="justify">
A continuación, se detalla la sintaxis lógica y estructural en formato de pseudocódigo estándar para cada uno de los tipos de condicionales explicados:
</p>

### Pseudocódigo: Estructura Condicional Simple
```text
Si (condicion_logica) Entonces
    // Bloque de instrucciones a ejecutar si la condición es Verdadera
FinSi
