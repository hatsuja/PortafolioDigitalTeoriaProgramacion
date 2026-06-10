
# <div align="center">Estructuras Condicionales</div>

---

## 1.1 ¿Qué son las Estructuras Condicionales?

<p align="justify">
Las estructuras condicionales (también conocidas como estructuras de bifurcación o selectivas) son instrucciones de control que permiten alterar el flujo lineal y secuencial de la ejecución de un programa siendo su propósito principal es evaluar una condición lógica o una expresión booleana que puede resultar únicamente en verdadero o falso y, en función de dicho resultado, desviar el camino del flujo para ejecutar un bloque específico de código.
</p>

<p align="justify">
En el ámbito del desarrollo de software, estas estructuras dotan a los algoritmos de la capacidad de tomar decisiones dinámicas en tiempo real en base a los datos de entrada proporcionados por el usuario o por el entorno físico de ejecución, evitando que el programa actúe siempre de la misma forma rígida.
</p>

## 1.2 Tipos de Condicionales

### A. Estructuras condicionales simples (`if`)
<p align="justify">
Evalúa una única condición lógica ya que si esta se cumple es verdadera, el programa ingresa y procesa las instrucciones delimitadas en su interior. En caso de que la condición no se cumpla seria falsa y el bloque interno es completamente ignorado y el compilador continúa con la ejecución lineal de la siguiente línea de código externa.
</p>

#### Pseudocódigo:
```
Si (condicion_logica) Entonces
    // Bloque de instrucciones a ejecutar si la condición es Verdadera
FinSi
```
#### Diagrama de flujo:

<div align="center">
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/2ad3813f-c34e-4a2a-aa52-a8d45b4710b6" />
</div>


### B. Estructuras condicionales dobles (`if else`)
<p align="justify">
Permite dividir el flujo del algoritmo en dos rutas alternativas ya que al evaluarse la expresión de control, si el resultado es verdadero, se procesa obligatoriamente el bloque del <code>if</code>; de lo contrario, si la expresión resulta ser falsa, el flujo se desvía sin excepción para ejecutar el bloque secundario definido bajo la palabra reservada <code>else</code> (sino).
</p>


#### Pseudocódigo:
```
Si (condicion_logica) Entonces
    // Bloque de instrucciones si la condición es Verdadera
Sino
    // Bloque de instrucciones alternativo si la condición es Falsa
FinSi
```
#### Diagrama de flujo:

<div align="center">
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/beca1b80-7a8c-4280-bb31-62ac11e16b62" />
</div>


### C. Estructuras condicionales múltiples ( `case` / `switch`)
**Estructura `case`, `switch`:** Sirve para evaluar el valor exacto de una única variable cuantitativa (generalmente de tipo entero o carácter). Compara dicho valor de forma directa contra una serie de casos preestablecidos (<code>case</code>). Si encuentra una coincidencia exacta, procesa ese bloque; opcionalmente incluye una sección por defecto (<code>default</code> o de otro modo) para manejar situaciones no previstas.


#### Pseudocódigo:
```
Según (variable_evaluada) Hacer
    Caso valor_1:
        // Instrucciones si variable_evaluada es estrictamente igual a valor_1
    Caso valor_2:
        // Instrucciones si variable_evaluada es estrictamente igual a valor_2
    De Otro Modo:
        // Instrucciones de escape si la variable no coincidió con ningún valor previo
FinSegun
```

#### Diagrama de flujo:

<div align="center">
<img width="810" height="307" alt="image" src="https://github.com/user-attachments/assets/d6c2271f-1925-4c2f-9b6b-b5bba8ba38c8" />
</div>

### D. Anidamiento de estructuras de Condicionales 
#### Estructura Condicional en Cascada(`if else if`)
**Estructura `if else if` (Anidada):** Se encarga de evaluar de forma ordenada y secuencial una serie de condiciones distintas ya que cuando una de las expresiones lógicas resulta verdadera, se ejecuta su respectivo bloque interno y el programa sale automáticamente de toda la estructura de control, omitiendo las validaciones restantes.

#### Pseudocódigo:
```
Si (condicion_1) Entonces
    // Instrucciones si la condicion_1 es Verdadera
Sino Si (condicion_2) Entonces
    // Instrucciones si la condicion_1 es Falsa y la condicion_2 es Verdadera
Sino
    // Instrucciones por defecto si ninguna de las condiciones previas se cumplió
FinSi
```

#### Diagrama de flujo:
<div align="center">
<img width="522" height="401" alt="image" src="https://github.com/user-attachments/assets/dd58d0a4-f31a-42fa-97b1-dad3bab131c9" />
</div>


---


<p align="center">
  <a href="https://github.com/hatsuja/PortafolioDigitalTeoriaProgramacion/blob/main/index.md">
    <b>📂 Ir al Índice Principal 📂</b>
  </a>
</p>

