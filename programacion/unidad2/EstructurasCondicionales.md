# <align="center">Estructuras Condicionales</align>

## ¿Qué son?
Las estructuras condicionales (también conocidas como estructuras de bifurcación o de toma de decisiones) son instrucciones de control que permiten alterar el flujo secuencial de un programa. Su función principal es evaluar una condición lógica (una expresión que da como resultado Verdadero o Falso) para determinar si se ejecuta o se omite un bloque específico de instrucciones. De este modo, el programa puede responder de manera dinámica e inteligente a diferentes entradas o escenarios de datos.

---

## Estructuras de Control

Las estructuras de control dirigen el orden en que se ejecutan las instrucciones de un programa. Sin ellas, el código se ejecutaría estrictamente de arriba hacia abajo (de forma lineal). Se clasifican en tres grandes grupos: secuenciales, condicionales y repetitivas.

### Estructura Algorítmicas Condicionales
Estas estructuras se basan en la evaluación de una propuesta lógica (relacional o booleana). El camino que tomará el flujo de ejecución depende enteramente de si se cumple o no la restricción evaluada.

---

## Condicionales

A continuación, se detallan y explican los tipos de estructuras condicionales utilizadas en la lógica de la programación, acompañadas por su respectiva representación en pseudocódigo.

### 1. Estructura Condicional Simple (Si ..Entonces)
Es la forma más básica de toma de decisiones. Evalúa una condición; si esta resulta ser **Verdadera**, se ejecuta el bloque de código contenido en su interior. Si la condición es **Falsa**, el programa ignora dicho bloque por completo y continúa con la instrucción inmediatamente posterior a la estructura.

#### Pseudocódigo:
```text
Si (condición_lógica) Entonces
    // Instrucciones que se ejecutan solo si la condición es Verdadera
FinSi
