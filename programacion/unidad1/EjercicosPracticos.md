# <p align="center">Ejercicios practicos</p>

---

<details>
  <summary>Contenidos</summary> 
  
  > Ejercicios en PSeInt
  
  > Ejercicios en C
</details>

---

<details>
  <summary>Lista de ejercicios</summary>

📂 [Presentación de la Unidad ](https://docs.google.com/presentation/d/1BXscIc91qjwGZLx_u-s0uHTUoemnmcoF/edit?slide=id.g381e014a9bd_0_148#slide=id.g381e014a9bd_0_148)

> Unidad 1. Elementos básicos de algoritmos y programas

</details>

---

## Ejercicios en PSeInt

---

* Un almacén requiere determinar cuánto cobrar por trabajos de pintura. Considere que se cobra por m2. Realice el algoritmo que le permita ir generando presupuestos para cada cliente.
<img width="1919" height="1009" alt="image" src="https://github.com/user-attachments/assets/b729d8f5-dfaa-4d7a-9a51-1b11dc6288ce" />

<div align="center">
  
### Prueba de escritorio

| metros | precio | total |
| :--- | :--- | :--- |
| 4| 20| 5*20 = 100| 

</div>

---

* Un alumno necesita calcular el promedio de sus 3 notas, cada una tiene una ponderación de: primera nota del 30%, segunda nota del 30% y tercera notas del 40%.

<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/2a9db45d-86b9-4e8e-bb95-c3cecbce0694" />

<div align="center">

### Prueba de escritorio

| Nota | Valor | Ponderación | Cálculo Parcial |
| :--- | :---: | :---: | :--- |
| Nota 1 | 7.0 | 30% | $7.0 \times 0.30 = 2.10$ |
| Nota 2 | 8.2 | 30% | $8.2 \times 0.30 = 2.46$ |
| Nota 3 | 6.7 | 40% | $6.7 \times 0.40 = 2.68$ |
| **Total** | | **100%** | **promedio: 7.24** |

</div>

---

* Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero. Para cada pedido, tiene que proporcionar las medidas de la tela en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo que determine cuántas pulgadas debe pedir con base en los metros que requiere (1 pulgada = 0.0254 m O 1 metro = 39.37 pulgadas)

<img width="1919" height="1005" alt="image" src="https://github.com/user-attachments/assets/67072538-cd2f-4d2c-bea7-96ae1be6148b" />

<div align="center">

### Prueba de escritorio

| Metros | Operación | Total Pulgadas |
| :---: | :---: | :---: |
| 20 m | $20 \times 39.37$ | 787.4 pulg. |

</div>

---

*Un productor de leche lleva el registro de lo que produce en litros, pero cuando entrega le pagan en galones. Realice un algoritmo que ayude al productor a saber cuánto recibirá por la entrega de su producción de un día (1 galón = 3.785 litros).

<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/44a21c36-4f1c-4d87-ac91-a392563a635e" />

<div align="center">

### Prueba de escritorio

| Litros Producidos | Operación (Litros / 3.785) | Total Galones | Precio por Galón | Total a Recibir |
| :---: | :---: | :---: | :---: | :---: |
| 5 | $5 / 3.785$ | 1.32 gal. | $20 | **$26.40** |

</div>

---

* Un estacionamiento requiere determinar el cobro que debe aplicar a las personas que lo utilizan. Considere que el cobro es con base en las horas que utiliza y que las fracciones de hora se toman como completas. Realice el algoritmo que permita determinar el cobro.

<img width="1919" height="993" alt="image" src="https://github.com/user-attachments/assets/a7ef6842-7ecd-4972-a3f3-3d47d850e414" />

<div align="center">

### Prueba de escritorio

| Horas | Precio por Hora | Operación | Total a Cobrar |
| :---: | :---: | :---: | :---: |
| 3  | $15 | $3 \times 15$ | **$45** |

</div>

---

* Realice el algoritmo para determinar cuánto dinero ahorra una persona en un año si considera que cada semana ahorra 15% de su sueldo (considere cuatro semanas por mes y que no cambia el sueldo).

<img width="1919" height="994" alt="image" src="https://github.com/user-attachments/assets/897ddd4c-d086-4076-8e60-3ec18969adc0" />

<div align="center">

###  Prueba de escritorio

| Sueldo Mensual | Ahorro Semanal (15%) | Ahorro Mensual ($\times 4$) | Total Ahorro Anual ($\times 12$) |
| :---: | :---: | :---: | :---: |
| $1000 | $150 | $600 | **$7,200** |

</div>

---

## Ejercicios en C

* Escribir un programa que lea un número entero y a continuación, visualice su doble y su triple.

<img width="1019" height="848" alt="image" src="https://github.com/user-attachments/assets/8d0bf9cf-90ab-4a7d-8f4f-2b0f83ddf278" />


<div align="center">

### Prueba de escritorio

| Número Ingresado | Cálculo Doble (x2) | Resultado Doble | Cálculo Triple (x3) | Resultado Triple |
| :---: | :---: | :---: | :---: | :---: |
| 2 | $2 \times 2$ | 4 | $2 \times 3$ | 6 |

</div>

---

* Escribir un programa para convertir una medida dada en pies a sus equivalentes en: a) yardas; b) pulgadas; c) centímetros; y d) metro. (1 pie: 12 pulgadas, 1 yarda= 3 pies, 1 pulgada= 2.54 cm, 1 metro= 100 cm). Leer el número de pies e imprimir el número de yardas, pies, pulgadas, centímetros y metros.

<img width="1063" height="921" alt="image" src="https://github.com/user-attachments/assets/7194699c-3374-4063-9671-7add0fdf731e" />

<div align="center">

### Prueba de escritorio

| Pies | Yardas ($\div 3$) | Pulgadas ($\times 12$) | Centímetros ($\text{pulg} \times 2.54$) | Metros ($\text{cm} / 100$) |
| :---: | :---: | :---: | :---: | :---: |
| 10 | 3.33 | 120.00 | 304.80 | 3.048 |

</div>

---

* Realice un programa que tomado una cantidad expresada en metros lo transforme a su equivalente en kilómetros, centímetros y milímetros.

<img width="995" height="883" alt="image" src="https://github.com/user-attachments/assets/14444bbd-6bea-4af3-9591-885f80ed969a" />

<div align="center">

### Prueba de escritorio

| Metros | Kilómetros ($\div 1000$) | Centímetros ($\times 100$) | Milímetros ($\times 1000$) |
| :---: | :---: | :---: | :---: |
| 5 | 0.005 km | 500 cm | 5000 mm |

</div>

---

* Realice un programa que permita calcular la aceleración que tiene un cuerpo al conocer su velocidad inicial y final (m/s) en un instante de tiempo.

<img width="1039" height="884" alt="image" src="https://github.com/user-attachments/assets/ba961279-e123-48e5-ab27-43e61f8145bd" />

<div align="center">

### Prueba de escritorio: Cálculo de Aceleración

| V. Inicial | V. Final | Tiempo | Operación | Aceleración |
| :---: | :---: | :---: | :---: | :---: |
| 10 m/s | 30 m/s | 4 s | $(30 - 10) / 4$ | 5.00 $m/s^2$ |

</div>

---

* Realice un programa que calcule la distancia de entre los puntos p1(x1,y1) y p2(x2,y2) considerando que d= ((X2-X1)^2+(Y2-Y1)^2)^ 1⁄2

<img width="1050" height="875" alt="image" src="https://github.com/user-attachments/assets/476531b2-dc87-4abc-96ee-975de33b60d5" />

<div align="center">

### Prueba de escritorio: Distancia entre dos puntos

| Punto 1 ($x_1, y_1$) | Punto 2 ($x_2, y_2$) | Diferencias al cuadrado | Suma | Raíz (Distancia) |
| :---: | :---: | :--- | :---: | :---: |
| (0, 0) | (3, 4) | $(3-0)^2 = 9$ y $(4-0)^2 = 16$ | $9 + 16 = 25$ | **5.00** |

</div>

---

*Realice un programa que descomponga un número ingresado por el usuario en su parte entera y decimal.

<img width="1039" height="893" alt="image" src="https://github.com/user-attachments/assets/e3f21f3a-d056-41e9-8463-1d455d74bf58" />

<div align="center">

### Prueba de escritorio: Separación de Parte Entera y Decimal

| Número Ingresado | Proceso Parte Entera | Resultado Entero | Proceso Parte Decimal | Resultado Decimal |
| :---: | :---: | :---: | :---: | :---: |
| 12.45 | `(int)12.45` | 12 | $12.45 - 12$ | **0.45** |

</div>

---

