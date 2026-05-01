# <p align="center">Algoritmo</p>

## ¿Qué es un algoritmo?
Un algoritmo es básicamente una receta o una lista de pasos que seguimos para resolver un problema o completar una tarea.

>**Por ejemplo, preparar un café:**
>>1. Pones agua a hervir.
>>2. Colocas el café en el filtro.
>>3. Viertes el agua caliente.
>>4. Sirves en una taza.

### Características principales:
* **Es ordenado:** Los pasos van uno tras otro.
* **Es preciso:** Cada paso es claro y no da lugar a dudas.
* **Tiene un final:** La tarea se termina.

---

## Clasificación de un algoritmo

### Cualitativos
Son aquellos que usamos con palabras, como una receta de cocina o las instrucciones para armar un mueble.

>**Ejemplo: Cambiar una bombilla (foco)**
>>1.Apagar el interruptor de la luz.
>>2.Colocar una escalera debajo de la lámpara.
>>3.Subir la escalera con cuidado.
>>4.Girar la bombilla vieja hacia la izquierda hasta que salga.
>>5.Colocar la bombilla nueva y girarla hacia la derecha hasta que ajuste.
>>6.Bajar de la escalera y encender el interruptor.

### Cuantitativos
Son los que utilizan cálculos numéricos y matemáticas para llegar a un resultado.

>**Ejemplo: Calcular el área de un triángulo**
>>1. Conocer la medida de la base (b).
>>2. Conocer la medida de la altura (h).
>>3. Multiplicar la base por la altura (b*h).
>>4. Dividir el resultado anterior entre 2.
>>5. El resultado final es el área (A).

En matemáticas se vería así:  
$$A = \frac{b \times h}{2}$$

---

## Estructura de un algoritmo
Un algoritmo se compone de 3 partes:

1. **Entrada (Input):** Es la información o los datos iniciales.
2. **Proceso:** Es el conjunto de pasos o cálculos que transforman los datos.
3. **Salida (Output):** Es el resultado final que se obtiene.

---
## <p align="center">Representación de un Algoritmo </p>

### Lenguaje Natural
Es la forma más sencilla utilizando nuestro propio idioma.
> *Ejemplo: "Primero pides el nombre del usuario, luego verificas si es mayor de edad y, si lo es, le permites el acceso".*

### Pseudocódigo
Es un punto medio entre nuestro idioma y el lenguaje de programación. Usamos herramientas como **PSeInt**.

**Estructura básica en PSeInt:**
`Algoritmo NombreDelPrograma
    // Aquí van las declaraciones y procesos
FinAlgoritmo]`

Ejemplo básico 
Este es un ejemplo de cómo se vería un programa completo:

```pseudocodigo
Algoritmo CalcularPromedio
    // 1. Entrada de datos
    Escribir "Por favor, ingresa la primera nota:"
    Leer nota1
    Escribir "Ingresa la segunda nota:"
    Leer nota2
    
    // 2. Proceso (Cálculo)
    promedio <- (nota1 + nota2) / 2
    
    // 3. Salida de resultados
    Escribir "Tu promedio final es: ", promedio
    
    // Condicional sencillo para dar apoyo
    Si promedio >= 7 Entonces
        Escribir "¡Felicidades! Has aprobado."
    Sino
        Escribir "No te desanimes, sigue practicando."
    FinSi
FinAlgoritmo
```
### Diagrrama de flujo
* **Un diagrama de flujo** es la representación gráfica de un algoritmo y utiliza símbolos estandarizados para mostrar visualmente el camino que siguen los datos y las decisiones que se toman durante un proceso
* **Óvalo (Inicio/Fin):** Indica dónde empieza y dónde termina el algoritmo. Todo diagrama debe tener solo uno de inicio y al menos uno de fin.
* **Paralelogramo (Entrada/Salida):** Se usa cuando el programa necesita pedir un dato al usuario (Leer) o mostrar un resultado (Escribir).
* **Rectángulo (Proceso):** Representa cualquier operación lógica o matemática (sumas, asignaciones, cálculos).
Rombo (Decisión): Representa una pregunta que solo tiene dos respuestas posibles: Sí/No o Verdadero/Falso. De aquí salen dos caminos distintos.
* **Flechas (Líneas de flujo):** Indican la dirección del proceso; conectan los símbolos y muestran qué paso sigue.

#### ***Prueba de escritorio***
La prueba de escritorio se utiliza para verificar si un algoritmo funciona correctamente 
<div align="center">

| Línea del Código | nota1 | nota2 | promedio |
| :--- | :---: | :---: | :---: |
| Escribir... | - | - | - |
| Leer nota1 | **9** | - | - |
| Escribir... | 9 | - | - |
| Leer nota2 | 9 | **8** | - |
| promedio <- ... | 9 | 8 | **8.5** |
| Escribir... | 9 | 8 | 8.5 |
| Si promedio >= 7 | 9 | 8 | 8.5 |
| Escribir... | 9 | 8 | 8.5 |

</div>


# <p align="center">Lenguajes de programación</p>
