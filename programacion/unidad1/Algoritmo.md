
# <p align="center">Algoritmo</p>

## ¿Qué es un algoritmo?
Un algoritmo es básicamente una receta o una lista de pasos que seguimos para resolver un problema o completar una tarea

>**Por ejemplo, preparar un café:**
>>1. Pones agua a hervir
>>2. Colocas el café en el filtro
>>3. Viertes el agua caliente
>>4. Sirves en una taza

### Características principales:
* **Es ordenado:** Los pasos van uno tras otro
* **Es preciso:** Cada paso es claro y no da lugar a dudas
* **Tiene un final:** La tarea se termina

---

## Clasificación de un algoritmo

### Cualitativos
Son aquellos que usamos con palabras, como una receta de cocina o las instrucciones para armar un mueble

>**Ejemplo: Cambiar una bombilla (foco)**
>>1.Apagar el interruptor de la luz
>>2.Colocar una escalera debajo de la lámpara
>>3.Subir la escalera con cuidado
>>4.Girar la bombilla vieja hacia la izquierda hasta que salga
>>5.Colocar la bombilla nueva y girarla hacia la derecha hasta que ajuste
>>6.Bajar de la escalera y encender el interruptor

### Cuantitativos
Son los que utilizan cálculos numéricos y matemáticas para llegar a un resultado

>**Ejemplo: Calcular el área de un triángulo**
>>1. Conocer la medida de la base (b)
>>2. Conocer la medida de la altura (h)
>>3. Multiplicar la base por la altura (b*h)
>>4. Dividir el resultado anterior entre 2
>>5. El resultado final es el área (A)

En matemáticas se vería así:  
$$A = \frac{b \times h}{2}$$

---

## Estructura de un algoritmo
Un algoritmo se compone de 3 partes:

1. **Entrada (Input):** Es la información o los datos iniciales
2. **Proceso:** Es el conjunto de pasos o cálculos que transforman los datos
3. **Salida (Output):** Es el resultado final que se obtiene

---
## <p align="center"> Representación de un Algoritmo </p>
### Lenguaje Natural
Es la forma más sencilla utilizando nuestro propio idioma
> *Ejemplo: "Primero pides el nombre del usuario, luego verificas si es mayor de edad y, si lo es, le permites el acceso"*

---


# <p align="center"> Progrmacion por bloques</p>

>La programación por bloques es una forma de aprender a programar de manera visual y muy sencilla
>Se usa en herramientas como Scratch, Blockly de Google o Code.org
## ¿Cómo funciona?
Cada bloque representa una instrucción o una regla lógica como "avanzar", "repetir" o "si pasa esto, haz aquello" y estos bloques están diseñados para encajar solo si la lógica es correcta. Si intentas poner una pieza donde no va, simplemente no encajará, lo que te ayuda a evitar errores desde el principio

## Caracteristicas:
* No se necesita memorizar palabras raras o sintaxis complicada
* Ayuda en cómo resolver un problema  antes de preocuparte por el lenguaje de programación técnico.
* Se usa mucho para crear juegos, animaciones y hasta para manejar robots sencillos.

<img width="1912" height="873" alt="image" src="https://github.com/user-attachments/assets/20255618-1670-4666-9a63-b982b58421ec" />

---

# <p align="center"> Pseudocódigo</p>

Es un punto medio entre nuestro idioma y el lenguaje de programación. Usamos herramientas como **PSeInt**

**Estructura básica en PSeInt:**
`Algoritmo NombreDelPrograma
    // Aquí van las declaraciones y procesos
FinAlgoritmo]`

Ejemplo básico 
Este es un ejemplo de cómo se vería un programa completo:

```
Algoritmo CalcularAreaTriangulo
	Definir base, altura, area Como Real
	Escribir "Ingresa la base del triángulo:"
	Leer base
	Escribir "Ingresa la altura del triángulo:"
	Leer altura
	// proceso
	area = (base * altura) / 2
	Escribir "El área del triángulo es: ", area
FinAlgoritmo
```

---
# <p align="center"> Diagrama de flujo</p>

Un diagrama de flujo es la representación gráfica de un algoritmo y utiliza símbolos estandarizados para mostrar visualmente el camino que siguen los datos y las decisiones que se toman durante un proceso

* **Óvalo (Inicio/Fin):** Indica dónde empieza y dónde termina el algoritmo. Todo diagrama debe tener solo uno de inicio y al menos uno de fin
* **Paralelogramo (Entrada/Salida):** Se usa cuando el programa necesita pedir un dato al usuario (Leer) o mostrar un resultado (Escribir)
* **Rectángulo (Proceso):** Representa cualquier operación lógica o matemática (sumas, asignaciones, cálculos)
* **Rombo (Decisión):** Representa una pregunta que solo tiene dos respuestas posibles: Sí/No o Verdadero/Falso. De aquí salen dos caminos distintos
* **Flechas (Líneas de flujo):** Indican la dirección del proceso; conectan los símbolos y muestran qué paso sigue

<img width="1078" height="1080" alt="image" src="https://github.com/user-attachments/assets/ffd8da73-efa1-419f-8856-33dbdfc9f2a9" />

---

# <p align="center">Elementos básicos de algoritmos y programas </p> 
  
## Datos e información
Un dato representa información  que la computadora procesa y almacena en su memoria

---

## Tipo de datos

<div align="center">

| Tipo de Dato | Descripción | Ejemplos |
| :--- | :--- | :--- |
| **Enteros (int)** | Números exactos sin decimales (positivos, negativos o cero) | `10`, `-5`, `0`, `1500` |
| **Reales (float/double)** | Números que incluyen una parte decimal | `3.14`, `0.5`, `-1.2` |
| **Lógicos (boolean)** | Valores que representan estados binarios | `Verdadero`, `Falso` |
| **Carácter (char)** | Un único símbolo, letra o número | `'A'`, `'@'`, `'7'`, `'+'` |
| **Cadena (string)** | Una secuencia o unión de varios caracteres | `"Hola mundo"`, `"Gato"`, `"1234"` |

</div>

---

## Identificadores

Son los nombres que les damos a los objetos en un programa. `Deben empezar con una letra o subguión, no tener espacios, ni caracteres especiales como la "ñ" o tildes`  

**Variables:** Su valor puede cambiar durante el programa. `Se recomienda usar la notación lowerCamelCase (ej. nombreUsuario)`  

**Constantes:** Su valor no cambia. Por buena práctica, `se escriben siempre en MAYÚSCULAS`

---

## Operaciones Básicas

<div align="center">

| Operación | Descripción | Símbolo / Ejemplo |
| :--- | :--- | :--- |
| **Asignación** | Se usa para darle un valor a una variable | `=` o `<-` |
| **Entrada (Lectura)** | Instrucción para que el usuario ingrese datos | `Leer variable` |
| **Salida (Escritura)** | Instrucción para mostrar resultados en pantalla | `Escribir "Resultado"` |
| **Comentarios** | Notas para el programador que la computadora ignora al ejecutar | `//` |

</div>

---

## Expresiones y Prioridad de Operadores

<div align="center">

| Orden de Prioridad | Categoría | Operadores | Descripción |
| :---: | :--- | :--- | :--- |
| 1 | **Agrupación** | `( )`, `[ ]`, `{ }` | Paréntesis y otros signos de agrupación |
| 2 | **Aritméticos (Altos)** | `^`, `**`, `sqrt()` | Potencia y raíz cuadrada |
| 3 | **Aritméticos (Medios)** | `*`, `/`, `mod`, `%` | Multiplicación, división y residuo (módulo) |
| 4 | **Aritméticos (Bajos)** | `+`, `-` | Suma y resta |
| 5 | **Relacionales** | `>`, `<`, `>=`, `<=`, `=`, `<>` | Comparaciones (mayor, menor, igual, diferente) |
| 6 | **Lógicos** | `NOT`, `AND`, `OR` | Negación, conjunción y disyunción |

</div>

---

## Prueba de escritorio
La prueba de escritorio se utiliza para verificar si un algoritmo funciona correctamente 

#### Ejemplo en PSeInt

```
Algoritmo CalcularAreaTriangulo
	Definir base, altura, area Como Real
	Escribir "Ingresa la base del triángulo:"
	Leer base
	Escribir "Ingresa la altura del triángulo:"
	Leer altura
	// proceso
	area = (base * altura) / 2
	Escribir "El área del triángulo es: ", area
FinAlgoritmo
```

### <div align="center"> Area de un triángulo </div>

Datos

Altura=3

Base=4

Area= 6

$$A = \frac{b \times h}{2}$$
<div align="center">

| Base | Altura | Area |
| :--- | :--- | :--- |
| 4| 6| $$A = \frac{4 \times 3}{2}$$ = 6| 

</div>

---



