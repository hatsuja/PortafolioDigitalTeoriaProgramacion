# Unidad 1: Algoritmos

## ¿Qué es un algoritmo?
Un algoritmo es básicamente una **receta** o una lista de pasos que seguimos para resolver un problema o completar una tarea.

**Ejemplo cotidiano: Preparar un café**
1. Pones agua a hervir.
2. Colocas el café en el filtro.
3. Viertes el agua caliente.
4. Sirves en una taza.

En la tecnología es exactamente lo mismo: son las instrucciones que le damos a una computadora para que sepa qué hacer, desde organizar una lista de nombres hasta mostrar páginas de internet.

### Características principales:
* **Es ordenado:** Los pasos van uno tras otro.
* **Es preciso:** Cada paso es claro y no da lugar a dudas.
* **Tiene un final:** La tarea siempre debe terminar.

---

## Clasificación de un algoritmo

### 1. Cualitativos
Son aquellos que usamos con **palabras**, como una receta de cocina o instrucciones para armar un mueble.

**Ejemplo: Cambiar una bombilla (foco)**
* Apagar el interruptor de la luz.
* Colocar una escalera debajo de la lámpara.
* Subir la escalera con cuidado.
* Girar la bombilla vieja hacia la izquierda hasta que salga.
* Colocar la bombilla nueva y girarla hacia la derecha hasta que ajuste.
* Bajar de la escalera y encender el interruptor.

### 2. Cuantitativos
Son los que utilizan **cálculos numéricos** y matemáticas para llegar a un resultado.

**Ejemplo: Calcular el área de un triángulo**
1. Conocer la medida de la base ($b$).
2. Conocer la medida de la altura ($h$).
3. Multiplicar la base por la altura ($b \times h$).
4. Dividir el resultado anterior entre 2.
5. El resultado final es el área ($A$).

En matemáticas se vería así:  
$$A = \frac{b \times h}{2}$$

---

## Estructura de un algoritmo
Un algoritmo se compone de 3 partes fundamentales:

1.  **Entrada (Input):** Es la información o los datos iniciales.
    * *Ejemplo:* Si quieres calcular la edad de alguien, la entrada es el año de nacimiento.
2.  **Proceso:** Es el conjunto de pasos o cálculos que transforman los datos.
    * *Ejemplo:* La resta: `año actual - año de nacimiento`.
3.  **Salida (Output):** Es el resultado final obtenido.
    * *Ejemplo:* La edad de la persona (ej. 20 años).

---

## Representación de un algoritmo

### 1. Lenguaje Natural
Es la forma más sencilla, utilizando nuestro propio idioma.
> *Ejemplo: "Primero pides el nombre del usuario, luego verificas si es mayor de edad y, si lo es, le permites el acceso".*

### 2. Pseudocódigo
Es un punto medio entre nuestro idioma y el lenguaje de programación. No tiene reglas tan estrictas como el código real, pero sigue una estructura lógica. Para esto, solemos usar herramientas como **PSeInt**.

**Estructura básica en PSeInt:**
```pseint
Algoritmo NombreDelPrograma
    // Aquí van las declaraciones y procesos
    Escribir "Hola, bienvenido"
FinAlgoritmo
