# Laboratorio09

Preguntas:
1.¿Qué es una coroutine en Kotlin y cómo se diferencia de un hilo
tradicional?
R//Las coroutines son un mecanismo de programación que permite escribir código asíncrono de manera
secuencial y estructurada en Kotlin. A diferencia de los hilos tradicionales, las coroutines son concurrencia
cooperativa, lo que significa que el programador tiene el control para decidir cuándo se suspende y reanuda.

2. ¿Cuál es la importancia de la suspensión en las coroutines y cómo se
implementa?
R//La suspensión en las coroutines de Android se refiere a la capacidad de suspender momentáneamente la
ejecución de una coroutine sin obstruir el main thread.Cuando se suspende una coroutine, el hilo que estaba
utilizando se libera para que otras coroutines o acciones puedan utilizarlo. Como resultado, es posible desarrollar
código asíncrono y no bloqueante que pueda manejar actividades largas o bloqueantes sin interferir con el hilo
principal de la interfaz de usuario o hacer que la aplicación sea inutilizable.

3. ¿Cuál es el propósito del Dispatcher en las coroutines y cómo se elige
uno adecuado para cada tarea?
R//La función de un Dispatcher es especificar en qué hilo (o hilos) se ejecutará una coroutine. Son sumamente
útiles ya que existen tareas de Input/Output de red o de archivos , que no pueden realizarse en el hilo principal.
os Dispatchers ofrecen varios contextos de subprocesos para diversas operaciones. Por ejemplo, el Dispatcher
Dispatchers.Main ejecuta coroutines en el hilo principal de la aplicación, que es también su hilo UI. Esto se puede
utilizar para actualizar la interfaz de usuario o llevar a cabo otras acciones que requieren la participación de la
interfaz de usuario.

4. ¿Cuál es el propósito y el uso de la función async en las coroutines?
R//Constructor utilizado para lanzar coroutines de manera asíncrona se obtiene el resultado
utilizando el objeto Deferred. El resultado se obtiene mediante la función await(). Y es útil cuando se
deben ejecutar tareas concurrentes y combinar los resultados.
