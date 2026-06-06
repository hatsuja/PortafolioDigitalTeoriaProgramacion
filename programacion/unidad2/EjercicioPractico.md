
# <div align="center">Ejercicio Practico</div>

---

## 3.1 Planteamiento del Problema

<p align="justify">
Se requiere un programa que permita gestionar el registro y procesamiento de las calificaciones académicas de un número indeterminado de estudiantes. El programa debe solicitar inicialmente la cantidad total de alumnos a evaluar y, de forma iterativa, recopilar las notas correspondientes a los cuatro componentes del modelo educativo vigente: <b>ACD</b> (Aprendizaje en Contacto con el Docente), <b>AA</b> (Aprendizaje Autónomo), <b>APE</b> (Aprendizaje Práctico Experimental) y <b>ES</b> (Examen de Fin de Ciclo).
</p>

<p align="justify">
Para garantizar la integridad y robustez de la aplicación, se deben incorporar mecanismos de validación que impidan el ingreso de valores incoherentes (la cantidad de estudiantes debe ser estrictamente mayor a 0 y todas las calificaciones individuales deben situarse obligatoriamente en el rango cerrado de 0 a 10 puntos). Una vez recopilados los datos válidos, el algoritmo debe calcular el aporte ponderado de cada nota según su peso porcentual, computar la Nota Final de cada alumno y determinar su equivalencia cualitativa mediante la siguiente escala académica institucional:
</p>

<ul>
    <li>Nota Final menor a 5.00: <b>Deficiente</b></li>
    <li>Nota Final entre 5.00 y menor a 7.00: <b>Regular</b></li>
    <li>Nota Final entre 7.00 y menor a 9.00: <b>Buena</b></li>
    <li>Nota Final entre 9.00 y 10.00: <b>Excelente</b></li>
</ul>

---

## 3.2 Análisis del Problema

<p align="justify">
Para estructurar la solución lógica de manera eficiente, se desglosa el comportamiento del sistema mediante una matriz de análisis técnico que define las entradas requeridas, las operaciones de procesamiento y las salidas esperadas:
</p>

<table align="center" border="1" cellpadding="8" style="border-collapse: collapse; width: 100%; max-width: 850px; background-color: #ffffff;">
    <thead>
        <tr style="background-color: #4A148C; color: #ffffff; text-align: center;">
            <th style="width: 30%;">Datos de Entrada</th>
            <th style="width: 40%;">Procesamiento / Fórmulas</th>
            <th style="width: 30%;">Datos de Salida</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left" valign="top">
                <b>Variables Cuantitativas:</b><br>
                <ul>
                    <li><code>est</code>: Cantidad total de estudiantes (Entero).</li>
                    <li><code>acd</code>: Nota del componente docente (Real, 0-10).</li>
                    <li><code>aa</code>: Nota del componente autónomo (Real, 0-10).</li>
                    <li><code>ape</code>: Nota del componente práctico (Real, 0-10).</li>
                    <li><code>es</code>: Nota del examen de fin de ciclo (Real, 0-10).</li>
                </ul>
            </td>
            <td align="left" valign="top">
                <b>1. Validación de Rangos:</b><br>
                • Asegurar <code>est > 0</code> mediante bucle <code>do-while</code>.<br>
                • Asegurar <code>nota >= 0 y nota <= 10</code> para cada componente académico.<br><br>
                <b>2. Cálculo de Ponderados Individuales:</b><br>
                • <code>acd = acd * 2.0</code> (Aporta 20% / 2 pts)<br>
                • <code>aa = aa * 2.0</code> (Aporta 20% / 2 pts)<br>
                • <code>ape = ape * 2.5</code> (Aporta 25% / 2.5 pts)<br>
                • <code>es = es * 3.5</code> (Aporta 35% / 3.5 pts)<br><br>
                <b>3. Cálculo de la Nota Final (Base 10):</b><br>
                • <code>nf = (acd + aa + ape + es) / 10.0</code><br><br>
                <b>4. Evaluación Cualitativa:</b><br>
                • Clasificación mediante condicionales anidadas (<code>if - else if - else</code>).
            </td>
            <td align="left" valign="top">
                <b>Resultados por Estudiante:</b><br>
                <ul>
                    <li>Identificador del estudiante en curso (<code>i</code>).</li>
                    <li>Valores individuales calculados para los ponderados ACD, AA, APE y ES.</li>
                    <li>Nota Final numérica ponderada (<code>nf</code>) formateada a dos decimales.</li>
                    <li>Categoría textual descriptiva del rendimiento alcanzado.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

---

## 3.3 Codificación en Lenguaje C

<p align="justify">
A continuación, se presenta la implementación del código fuente completamente depurado, funcional y estructurado bajo las directrices académicas solicitadas:
</p>

```c
#include <stdio.h>

int main() {
    // Declaración de variables para almacenar calificaciones y nota final
    float acd, aa, ape, es, nf;
    // Variables de control: cantidad total de estudiantes y contador del bucle
    int est, i;
    
    // ==========================================
    // GESTIÓN DE ENTRADA Y VALIDACIÓN INICIAL
    // ==========================================
    // Bucle do-while para asegurar que la cantidad de estudiantes sea válida
    do {
        printf("Ingresa el numero de estudiantes: ");
        scanf("%i", &est);
        // Validación: el número de estudiantes debe ser estrictamente mayor a cero
        if (est <= 0) {
            printf("Error, el numero debe ser mayor a 0.\n");
        }
    } while (est <= 0); // Repetir si el dato ingresado es incorrecto
    
    // ==========================================
    // ESTRUCTURA REPETITIVA PRINCIPAL (CICLO FOR)
    // ==========================================
    // Procesa de forma iterativa las calificaciones de cada estudiante individualmente
    for (i = 1; i <= est; i++) {
        
        // --- Validación y lectura del componente ACD ---
        do {
            printf("Ingrese la nota ACD del estudiante %i: ", i);
            scanf("%f", &acd);
            // Validar que la nota se encuentre en el rango permitido de 0 a 10
            if (acd < 0 || acd > 10) {
                 printf("Error no esta el rango (0-10).\n");
            }
        } while (acd < 0 || acd > 10); // Re solicita la nota hasta que sea correcta
        
        // --- Validación y lectura del componente AA ---
        do {
            printf("Ingrese la nota AA del estudiante %i: ", i);
            scanf("%f", &aa);
            // Validar que la nota se encuentre en el rango permitido de 0 a 10
            if (aa < 0 || aa > 10){ 
                 printf("Error no esta el rango (0-10).\n");
             }        
        } while (aa < 0 || aa > 10); // Re solicita la nota hasta que sea correcta
        
        // --- Validación y lectura del componente APE ---
        do {
            printf("Ingrese la nota APE del estudiante %i: ", i);
            scanf("%f", &ape);
            // Validar que la nota se encuentre en el rango permitido de 0 a 10
            if (ape < 0 || ape > 10){
                printf("Error no esta el rango (0-10).\n");
            }
        } while (ape < 0 || ape > 10); // Re solicita la nota hasta que sea correcta
        
        // --- Validación y lectura del componente ES ---
        do {
            printf("Ingrese la nota ES del estudiante %i: ", i);
            scanf("%f", &es);
            // Validar que la nota se encuentre en el rango permitido de 0 a 10
            if (es < 0 || es > 10){
                printf("Error no esta el rango (0-10).\n");
            }
        } while (es < 0 || es > 10); // Re solicita la nota hasta que sea correcta
        
        // ==========================================
        // PROCESAMIENTO Y CÁLCULO DE PONDERADOS
        // ==========================================
        acd = acd * 2;     // Cálculo del aporte correspondiente al 20% de la nota final
        aa = aa * 2;       // Cálculo del aporte correspondiente al 20% de la nota final
        ape = ape * 2.5;   // Cálculo del aporte correspondiente al 25% de la nota final
        es = es * 3.5;     // Cálculo del aporte correspondiente al 35% de la nota final
        
        // Cálculo general de la Nota Final (nf) promediada sobre 10 puntos
        nf = (acd + aa + ape + es) / 10;
        
        // ==========================================
        // PRESENTACIÓN DE RESULTADOS (SALIDA)
        // ==========================================
        printf("\nResultados del estudiante %i:\n", i);
        printf("  El ponderado de nota ACD es: %.2f\n", acd);
        printf("  El ponderado de tu nota AA es: %.2f\n", aa);
        printf("  El ponderado de tu nota APE es: %.2f\n", ape);
        printf("  El ponderado de tu nota ES es: %.2f\n", es);
        
        // Estructuras condicionales anidadas para determinar la cualidad cualitativa de la nota
        if (nf < 5) {
            // Condición para rendimiento Deficiente
            printf("  La nota es deficiente tiene %.2f\n", nf);
        } else if (nf >= 5 && nf < 7) {
            // Condición para rendimiento Regular
            printf("  La nota es regular tiene %.2f\n", nf);
        } else if (nf >= 7 && nf < 9) {
            // Condición para rendimiento Bueno
            printf("  La nota es buena tiene %.2f\n", nf);
        } else {
            // Condición por descarte para rendimiento Excelente (entre 9 y 10)
            printf("  La nota es excelente tiene %.2f\n", nf);
        }
    } 
    
    // Retorno de control exitoso al sistema operativo
    return 0;
}
```
