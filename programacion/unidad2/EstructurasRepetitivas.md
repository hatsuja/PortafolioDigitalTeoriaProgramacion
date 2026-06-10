
# <div align="center">Estructuras Repetitivas</div>

---

## 2.1 ¿Qué son las Estructuras Repetitivas?

<p align="justify">
Las estructuras repetitivas son conocidas como bucles, ciclos o estructuras de iteración y estas son instrucciones de control que permiten ejecutar un bloque específico de código múltiples veces y la repetición se mantiene activa de forma cíclica mientras una condición lógica o expresión booleana se evalúe como verdadera, o hasta que se alcance un número predeterminado de iteraciones.
</p>


## 2.2 Tipos de Estructuras Repetitivas

<p align="justify">
Dependiendo del momento en que se evalúe la condición de control y de si se conoce o no de antemano el número exacto de iteraciones, los bucles se clasifican en las siguientes categorías:
</p>

### A. Estructura Mientras (`while`)
<p align="justify">
Es una estructura de pre-prueba. Esto significa que evalúa la condición lógica antes de permitir el ingreso al bloque de código. Si la condición es verdadera, ejecuta las instrucciones en su interior y vuelve a evaluar; si es falsa desde la primera comprobación, el bucle no se ejecuta ni una sola vez. Es ideal cuando el número de repeticiones depende de factores externos variables durante la ejecución.
</p>

#### Pseudocódigo:
```
Mientras (condicion_logica) Hacer
    // Bloque de instrucciones a repetir
    // (Debe incluir la modificación de la variable de control)
FinMientras
```

#### Diagrama de flujo:

<div align="center">
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/f0f8708f-b31e-4bf2-af25-c3d38682a45d" />
</div>

### B. Estructura Hacer .. Mientras / Repetir .. Hasta (`do while`)
<p align="justify">
Es una estructura en el que la condición de control se evalúa al final de la iteración lo que garantiza que el bloque de instrucciones interno se ejecutará <b>al menos una vez</b>, sin importar si la condición es falsa desde el principio incluso esta estructura es utilizada para la validación de datos de entrada por ejemplo de asegurar un rango de 0 a X.
</p>

#### Pseudocódigo:
```
Repetir
    // Bloque de instrucciones a ejecutar al menos una vez
    // (Debe incluir la modificación de la variable de control)
Mientras (condicion_logica)
```

#### Diagrama de flujo:

<div align="center">
<img width="507" height="502" alt="image" src="https://github.com/user-attachments/assets/9413b6a2-5524-43c1-9d3f-94691fe3a452" />
</div>



### C. Estructura Para (`for`)
<p align="justify">
Es una estructura de control especializada en la iteración contada y se utiliza cuando se conoce  el número de veces que se debe repetir el ciclo antes de que este inicie inclusp integra en una sola línea de tres componentes esenciales: la inicialización de una variable contador, la condición de parada o límite, y la expresión de incremento o decremento que actualiza el contador tras cada iteración.
</p>

#### Pseudocódigo:
```
Para variable_contador <- valor_inicial Hasta valor_final Con Paso incremento Hacer
    // Bloque de instrucciones que se ejecutan de forma contada
FinPara
```

#### Diagrama de flujo:

<div align="center">
<img width="453" height="322" alt="image" src="https://github.com/user-attachments/assets/b0ab24eb-64d7-4bef-973f-cf99f09188e9" />
</div>


### D. Anidamiento de estructuras repetitivas
<p align="justify">
El anidamiento ocurre cuando se coloca una estructura repetitiva (bucle interno) dentro del cuerpo de instrucciones de otra estructura repetitiva (bucle externo) y por cada iteración única que realiza el ciclo externo, el ciclo interno ejecuta su secuencia de repeticiones completa de principio a fin.
</p>

<div align="center">
<img width="1121" height="423" alt="image" src="https://github.com/user-attachments/assets/5d32155e-32f0-4600-82af-c98f8a049551" />
</div>

#### Pseudocódigo:
```
Para i <- 1 Hasta limite_externo Hacer
    // Instrucciones del bucle externo
    Para j <- 1 Hasta limite_interno Hacer
        // Instrucciones del bucle interno (se ejecutan completamente por cada 'i')
    FinPara
FinPara
```
#### Diagrama de flujo:
<div align="center">
<img width="287" height="527" alt="image" src="https://github.com/user-attachments/assets/760ab4f7-8a17-459c-8343-af98487242e9" />
</div>

---

<p align="center">
  <a href="https://github.com/hatsuja/PortafolioDigitalTeoriaProgramacion/blob/main/index.md">
    <b>📂 Ir al Índice Principal 📂</b>
  </a>
</p>


