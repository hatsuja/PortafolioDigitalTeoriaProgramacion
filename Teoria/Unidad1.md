# <span style="color: #003366;">Unidad 1: Fundamentos de Programación</span>

## <span style="color: #2e6c80;">Algoritmo</span>

### ¿Que es un algoritmo?
Un algoritmo es básicamente una receta o una lista de pasos que seguimos para resolver un problema o completar una tarea. Por ejemplo, preparar un café:

*   Pones agua a hervir.
*   Colocas el café en el filtro.
*   Viertes el agua caliente.
*   Sirves en una taza.

Esta serie de pasos es un algoritmo y en la tecnología es lo mismo ya que son las instrucciones que le damos a una computadora para que sepa exactamente qué hacer, desde organizar una lista de nombres o mostrar paginas de internet.

**Características principales:**
*   **Es ordenado:** Los pasos van uno tras otro.
*   **Es preciso:** Cada paso es claro y no da lugar a dudas.
*   **Tiene un final:** la tarea se termina.

---

## <span style="color: #2e6c80;">Clasificación de un algoritmo</span>

### Cualitativos
Son aquellos que usamos con palabras, como una receta de cocina o las instrucciones para armar un mueble.

**Ejemplo: Cambiar una bombilla foco**
1. Apagar el interruptor de la luz.
2. Colocar una escalera debajo de la lámpara.
3. Subir la escalera con cuidado.
4. Girar la bombilla vieja hacia la izquierda hasta que salga.
5. Colocar la bombilla nueva y girarla hacia la derecha hasta que ajuste.
6. Bajar de la escalera y encender el interruptor.

### Cuantitativos
Son los que utilizan cálculos numéricos y matemáticas para llegar a un resultado.

**Ejemplo: Calcular el área de un triángulo**
1. Conocer la medida de la base (b).
2. Conocer la medida de la altura (h).
3. Multiplicar la base por la altura (b*h).
4. Dividir el resultado anterior entre 2.
5. El resultado final es el área (A).

En matemáticas se vería así:
$$A = \frac{b \times h}{2}$$

---

## <span style="color: #2e6c80;">Estructura de un algoritmo</span>

Un algoritmo de compone de 3 partes:

1. **Entrada (Input):** Es la información o los datos iniciales que necesita el algoritmo para empezar a trabajar. Sin estos datos, el proceso no tiene sobre qué actuar.
   * *Ejemplo:* Si quieres calcular la edad de alguien, la entrada sería el año de nacimiento.

2. **Proceso:** Es el conjunto de pasos, cálculos u operaciones que el algoritmo realiza con los datos de entrada para transformarlos. Es el "corazón" del algoritmo.
   * *Ejemplo:* Siguiendo el caso de la edad, el proceso sería la resta: año actual menos año de nacimiento.

3. **Salida (Output):** Es el resultado final que se obtiene una vez que el proceso ha terminado. Es la respuesta al problema inicial.
   * *Ejemplo:* El resultado de la resta, que sería la edad de la persona (por ejemplo, 20 años).

---

## <span style="color: #2e6c80;">Representación de un algoritmo</span>

### 1. Lenguaje Natural
Es la forma más sencilla utilizando nuestro propio idioma para describir los pasos uno por uno.
* *Ejemplo:* "Primero pides el nombre del usuario, luego verificas si es mayor de edad y, si lo es, le permites el acceso".

### 2. Pseudocódigo
Es un punto medio entre nuestro idioma y el lenguaje de programación ya que no tiene reglas tan estrictas como el código, pero sigue una estructura lógica. Existen varios programas de seudocódigo por ejemplo el **PSeInt**.

**Estructura básica de PSeInt:**
```cpp
Algoritmo NombreDelPrograma
    // Aquí van las declaraciones y procesos
FinAlgoritmo
