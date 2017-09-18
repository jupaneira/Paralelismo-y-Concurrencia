# Paralelismo-y-Concurrencia

## Hilos 
Ofrecen paralelismo en la ejecución del código a nivel de un mismo proceso <br/>
Procesos livianos (cuentan con sus propios registros y pilas)
La clase que modela los hilos en Java, se llama **Thread**

### Thread 
Atributos 

1. *Identificador* = níumero que identifica cada hilo. Inmutable durante la vida del thread y reutilizable luego de su terminación.
2. *Nombre* = genreado automáticamente por la JVM (puede modificarse)
3. *Prioridad* = Entero del 1 al 10
4. *Estado* = estado de ejecución del hilo (6 posibles estados)

Thread posee un método **run** abstracto. 

### Thread Safety 

Para garantizar que una clase sea Thread safety, se debe asegurar que al ser corrida por múltiples threads, el estado interno (sus atributos) mantengan los valores esperados al ejecutar cualquiera de sus métodos. 

*clases seguras*

Clases que no tienen estado. (No tiene atributos)
Clases inmutables (Tienen atributos pero no pueden ser modificados)
Clases que confinan sus métodos y atributos a un solo Thread



