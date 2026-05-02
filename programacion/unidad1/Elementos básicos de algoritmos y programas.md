# <p align="center">Elementos básicos de algoritmos y programas </p> 
  
## Datos e información
Un dato representa información  que la computadora procesa y almacena en su memoria

---

## Tipo de datos

<div align="center">

| Tipo de Dato | Descripción | Ejemplos |
| :--- | :--- | :--- |
| **Enteros (int)** | Números exactos sin decimales (positivos, negativos o cero). | `10`, `-5`, `0`, `1500` |
| **Reales (float/double)** | Números que incluyen una parte decimal. | `3.14`, `0.5`, `-1.2` |
| **Lógicos (boolean)** | Valores que representan estados binarios. | `Verdadero`, `Falso` |
| **Carácter (char)** | Un único símbolo, letra o número. | `'A'`, `'@'`, `'7'`, `'+'` |
| **Cadena (string)** | Una secuencia o unión de varios caracteres. | `"Hola mundo"`, `"Gato"`, `"1234"` |

</div>

---

## Identificadores

Son los nombres que les damos a los objetos en un programa. `Deben empezar con una letra o subguión, no tener espacios, ni caracteres especiales como la "ñ" o tildes.`  

**Variables:** Su valor puede cambiar durante el programa. `Se recomienda usar la notación lowerCamelCase (ej. nombreUsuario).`  

**Constantes:** Su valor no cambia. Por buena práctica, `se escriben siempre en MAYÚSCULAS.`

---

## Operaciones Básicas

<div align="center">

| Operación | Descripción | Símbolo / Ejemplo |
| :--- | :--- | :--- |
| **Asignación** | Se usa para darle un valor a una variable. | `=` o `<-` |
| **Entrada (Lectura)** | Instrucción para que el usuario ingrese datos. | `Leer variable` |
| **Salida (Escritura)** | Instrucción para mostrar resultados en pantalla. | `Escribir "Resultado"` |
| **Comentarios** | Notas para el programador que la computadora ignora al ejecutar. | `//` |

</div>

---

## Expresiones y Prioridad de Operadores

<div align="center">

| Orden de Prioridad | Categoría | Operadores | Descripción |
| :---: | :--- | :--- | :--- |
| 1 | **Agrupación** | `( )`, `[ ]`, `{ }` | Paréntesis y otros signos de agrupación. |
| 2 | **Aritméticos (Altos)** | `^`, `**`, `sqrt()` | Potencia y raíz cuadrada. |
| 3 | **Aritméticos (Medios)** | `*`, `/`, `mod`, `%` | Multiplicación, división y residuo (módulo). |
| 4 | **Aritméticos (Bajos)** | `+`, `-` | Suma y resta. |
| 5 | **Relacionales** | `>`, `<`, `>=`, `<=`, `=`, `<>` | Comparaciones (mayor, menor, igual, diferente). |
| 6 | **Lógicos** | `NOT`, `AND`, `OR` | Negación, conjunción y disyunción. |

</div>

---

## Prueba de escritorio
La prueba de escritorio se utiliza para verificar si un algoritmo funciona correctamente 

### Ejemplo en PSeInt

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

<div align="center"> Area de un triángulo </div>

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




