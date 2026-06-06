<div align="center">
  
# Reflexión Crítica
</div>

La creación de este simulador de caja registradora permitió llevar a la práctica conceptos estructurales de la programación lógica y el flujo de control algorítmico. El diseño del programa demuestra cómo la combinación de estructuras cíclicas iterativas y condicionales anidadas logra modelar un escenario real de transacciones comerciales de manera automatizada. El aspecto más valioso del ejercicio radica en la arquitectura del software para anticipar las decisiones del usuario: desde la asignación de un presupuesto inicial hasta la adición progresiva de ítems, el código actúa como un filtro constante que asegura la integridad de los datos financieros calculados. Esto resalta que programar no consiste únicamente en escribir instrucciones secuenciales, sino en diseñar un entorno seguro y predecible capaz de procesar variables dinámicas sin corromper el estado final del sistema, garantizando que el balance final (`saldo_restante`) coincida exactamente con la auditoría de los gastos acumulados.

### Principales Dificultades Encontradas

A nivel técnico, el mayor desafío consistió en la correcta implementación y sincronización de los ciclos que validan las entradas de datos. En particular, estructurar el bucle `do-while` interno para rechazar precios negativos sin interrumpir abruptamente la sesión general de compras requirió un manejo muy preciso de los ámbitos de control. Asimismo, coordinar los mecanismos de salida forzada (`break`) introdujo una capa de complejidad notable; gestionar el momento exacto en el que el usuario digita `0` para finalizar voluntariamente, frente a la interrupción automática cuando se excede el presupuesto disponible, exigió un diseño riguroso en las estructuras
