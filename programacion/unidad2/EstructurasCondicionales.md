<h1 align="center">Estructuras Condicionales</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Teoría%20de%20la%20Programación-Unidad%202-purple?style=for-the-badge" alt="Unidad 2">
</p>

## ¿Qué son las Estructuras Condicionales?

Las **estructuras condicionales** (también conocidas como estructuras de decisión o selectivas) son instrucciones de control que permiten bifurcar el flujo de ejecución de un programa basándose en el cumplimiento de una condición lógica. 

El programa evalúa una expresión booleana (cuyo resultado solo puede ser **Verdadero** o **Falso**) mediante operadores relacionales o lógicos. Dependiendo del resultado de esta evaluación, el flujo toma un camino u otro, permitiendo que el software tome decisiones en tiempo real en lugar de ejecutarse de forma estrictamente lineal.

---

## Estructuras de Control

En la ciencia de la computación, las estructuras de control determinan el orden en el que se ejecutan las instrucciones de un algoritmo. Se dividen fundamentalmente en tres grandes bloques:
1. **Secuenciales:** Ejecución paso a paso en orden descendente.
2. **Condicionales o Selectivas:** Bifurcan el flujo según una condición.
3. **Repetitivas o Iterativas:** Repiten un bloque de instrucciones mediante bucles.

### Estructura Algorítmicas Condicionales
Estas estructuras se especializan en evaluar situaciones variables. Su objetivo principal es direccionar el comportamiento del programa basándose en los datos de entrada o cálculos intermedios generados durante la ejecución.

---

## Condicionales: Tipos y Representación en Pseudocódigo

A continuación se detallan las distintas variantes de las estructuras condicionales aplicadas en la lógica de programación:

### 1. Estructura Condicional Simple (Si... Entonces)
Es el tipo más básico de decisión. Evalúa una condición y, únicamente si el resultado es **Verdadero**, ejecuta el bloque de código interno. Si el resultado es **Falso**, ignora las instrucciones asociadas y continúa de largo con el resto del programa.

#### Representación en Pseudocódigo:
```text
Si (condición_lógica) Entonces
    // Bloque de instrucciones que se ejecuta solo si es Verdadero
FinSi
