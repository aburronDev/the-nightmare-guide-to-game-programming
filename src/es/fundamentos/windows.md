# No uses Windows

> Disclaimer:
>
> No voy a tratar de convencerte de que dejes de usar Windows, pero si estás leyendo esta guía no entiendo por qué todavía sigues usándolo.

Dejando a un lado la típica pelea de foroadictos sobre cual es el mejor sistema operativo...

Te voy a contar un cuento no tan infantil para programadores con el que espero que te sientas identificado:

> <center>
> <h1>Pepe el Programas</h1>
> </center>
> 
> Érase una vez un joven programador de videojuegos llamado Pepe que vivia en un piso de estudiantes en Madrid, pagado con el ahorro de sus padres.
>
> Sus compañeros de piso siempre se iban de fiesta los fines de semanas, pero Pepe siempre se quedaba en su cuarto programando con Unity para seguir aprendiendo. Es por esto que sus compañeros le llamaban Pepe el Programas, para meterse con él.
>
> Un día Pepe recibió un correo donde le aceptaban para trabajar en un videojuego de móviles parecido a Candy Crush, pero con un sistema de ligas y torneos semanales. Pepe tenía experiencia programando videojuegos de móviles por su cuenta, pero no había publicado ninguno en Google Play ni en App Store.
>
> Al día siguiente llegó a la oficina para empezar a trabajar, y tras conocer a sus compañeros le presentan la primera tarea: Solucionar un bug en el que la puntuación de un jugador no aumenta en el menú de torneo al completar un nivel.
>
> Pepe no tenía ni idea por donde empezar, de hecho no sabía ni lo que era un servidor. El programador jefe le explica que un servidor es un ordenador como otro cualquiera que tienen en la oficina, con la diferencia de que siempre está encendido.
>
> Pepe pregunta donde está el ordenador, para sentarse allí y trabajar, pero de repente se hizo un silencio incómodo mientras el resto de sus compañeros le miraban sin saber que decirle. El programador jefe le pregunta para qué necesita saber donde está el servidor, cuando puede conectarse por SSH.
>
> Como era de esperar, Pepe no estaba entendiendo nada de lo que le decian, pero les dijo que iba a ponerse a ello y les avisaba si no sabía como avanzar. Pasado unas horas, el programador jefe se pasó por su mesa para ver como lo llevaba. Vio que se había instalado PuTTY, pero no sabía como tenía que usarlo.
>
> El programador jefe se sienta junto a él y le dice que abra la consola de comandos, y se conecte con el comando ssh a la ip del servidor que hay en la red local.
>
> Pepe estaba alucinando porque es la primera vez que veia algo así, pero esa ilusión se conventiría rapidamente en desesperación al darse cuenta de que no tenía una interfaz gráfica, y que tenía que aprender a moverse entre directorios para acceder a la base de datos, y crear una columna para la puntuación que se había borrado por error...
>
> Definitivamente, Pepe era mucho más feliz programando en Unity.
>
> Aún así, Pepe se ha dado cuenta de que un programador necesita de unos conocimientos generales que no se consiguien aprendiendo sólo programación de videojuegos.

¿Que te ha parecido la historia de Pepe?

Aunque sea un ejemplo de un caso hipotético, te puedo contar la misma historia con diferentes situaciones que se pueden dar:

> Pepe ha creado una ruta `/user/rewards` en el servidor que se encarga de dar las recompensas a los 30 jugadores con mayor puntuación en el torneo, pero tiene que subir los cambios al repositorio de gitlab y nunca ha usado el comando git a través de un terminal.

> Pepe está teniendo un bug que no consigue identificar, debido a que sólo ocurre cuando hace la build del juego y lo prueba en su móvil.
>
> Podría hacer debugging con `adb logcat -s Unity`, pero Pepe no sabe como usar un terminal, así que pierde el día entero haciendo builds a base de prueba y error hasta encontrar la solución sin saber cómo.

Ahora que te he expuesto varios casos donde vas a necesitar un terminal, quizás quieras darle un intento y ahorrarte la sorpresa, si no te la has llevado ya.

Si aún así sigues sin ver la necesidad de usarlo, no te preocupes, porque estoy a punto de desvelarte el lenguaje de programación con el que vamos a empezar en esta guía que tanto amas pero al mismo tiempo odias.