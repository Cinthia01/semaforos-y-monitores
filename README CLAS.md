# Concurrencia y Paralelismo
**SEMAFOROS Y MONITORES**
**Matricula** 58807  
**Alumno:** TREJO MOO CINTHIA GUADALUPE  


## REFERENCIA DEL TEMA

•	                **Semáforos y Monitores en Concurrencia y Paralelismo**

En los sistemas concurrentes y paralelos, la sincronización entre procesos o hilos es fundamental para evitar problemas como condiciones de carrera, inconsistencias en los datos y bloqueos. Dos mecanismos ampliamente utilizados para gestionar esta sincronización son los semáforos y los monitores.
Un semáforo es una variable entera que se utiliza para controlar el acceso a recursos compartidos mediante dos operaciones atómicas: wait (también llamada P o down) y signal (V o up). La operación wait decrementa el valor del semáforo; si el valor es cero, el proceso que intenta acceder al recurso se bloquea hasta que otro proceso libere el semáforo. La operación signal incrementa el valor y puede despertar procesos bloqueados.
Existen semáforos binarios, que solo toman valores 0 o 1 y garantizan exclusión mutua, y semáforos contadores, que permiten controlar el acceso a múltiples instancias de un recurso. Los semáforos son herramientas flexibles y potentes para coordinar la ejecución de procesos en sistemas donde varios hilos compiten por recursos limitados.
Por otro lado, los monitores son una abstracción de alto nivel que encapsula variables compartidas, procedimientos y mecanismos de sincronización. A diferencia de los semáforos, los monitores garantizan automáticamente la exclusión mutua, permitiendo que solo un proceso esté activo dentro del monitor a la vez. 
Además, utilizan variables de condición para que los procesos puedan esperar y ser notificados dentro del monitor, facilitando la coordinación entre ellos. Esto simplifica la programación concurrente al ocultar detalles complejos de sincronización y reducir errores.
En el contexto de la concurrencia, donde múltiples tareas progresan simultáneamente pero no necesariamente al mismo tiempo, y el paralelismo, que implica la ejecución simultánea real en múltiples procesadores o núcleos, tanto semáforos como monitores son esenciales para evitar conflictos y asegurar la correcta interacción entre procesos. Sin estos mecanismos, los sistemas podrían experimentar errores como condiciones de carrera, inconsistencias en datos o bloqueos.

•	**Conclusión sobre semáforos y monitores**

Los semáforos permiten controlar el acceso a recursos compartidos mediante un contador que indica cuándo un proceso puede entrar o debe esperar, mientras que los monitores ofrecen una forma más estructurada y segura de garantizar que solo un proceso acceda a una sección crítica, facilitando la coordinación mediante variables de condición. Ambos mecanismos ayudan a evitar problemas comunes en la concurrencia y el paralelismo, como las condiciones de carrera o bloqueos, asegurando que los procesos trabajen de manera ordenada y sin interferencias.



