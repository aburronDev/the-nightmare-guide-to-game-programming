# No uses Windows

> Disclaimer:
>
> No voy a tratar de convencerte de que dejes de usar Windows, pero deberías considerar las ventajas de cambiar a otro sistema operativo.

Dejando a un lado la típica pelea de foroadictos sobre cuál es el mejor sistema operativo, es hora de que leas una pequeña historia con la que te sentirás identificado:

> <center>
> <h1>Pepe el Programador</h1>
> </center>
> 
> Érase una vez un de videojuegos llamado Pepe, que vivía en un piso para estudiantes en Madrid, pagado con el ahorro de sus padres.
>
> Mientras sus compañeros de piso se iban de fiesta todos los fines de semanas, Pepe permanecía diligente en su cuarto programando con Unity para seguir aprendiendo. Además, era víctima de múltiples memes, algunos bastante buenos.
>
> Un día, Pepe fue aceptado para trabajar en un videojuego de móviles parecido a Candy Crush, que poseía un sistema de ligas y torneos semanales. Pepe tenía experiencia programando videojuegos de móviles por su cuenta, pero no había publicado ninguno en Google Play ni en la App Store.
>
> Al día siguiente, cuando llegó a la oficina para comenzar a trabajar y, tras conocer a sus compañeros, le presentaron su primera tarea: Solucionar un bug en el que el servidor no guarda la puntuación obtenida de un jugador al completar un nivel.
>
> Pepe no tenía ni idea de por dónde empezar; de hecho, no sabía ni lo que era un servidor. El programador jefe le explicó que un servidor es un ordenador como cualquier otro, con la diferencia de que siempre está encendido.
>
> Tan pronto como Pepe preguntó dónde se encontraba dicho ordenador, el resto de compañeros le miraron sin saber qué decir. El programador jefe le preguntó por qué necesitaba saber dónde estaba el servidor, si podía conectarse por SSH.
>
> Como era de esperar, Pepe no entendió nada, aunque se puso con ello. Pasadas unas horas, el programador jefe se pasó por su mesa para ver cómo lo llevaba. Para su sorpresa, comprobó que había instalado PuTTY, pero no sabía cómo usarlo.
>
> El programador jefe se sentó junto a él y le pidió que abriera la consola de comandos para conectarse a la ip del servidor de la red local con el comando ssh.
>
> Pepe estaba alucinando, ya que era la primera vez que veía algo así; no obstante, esa ilusión pronto se convertiría en desesperación al darse cuenta de que no poseía una interfaz gráfica, por lo que era necesario aprender a moverse entre los directorios para acceder a la base de datos, y crear una columna para la puntuación que se había borrado por error...
>
> Definitivamente, Pepe era mucho más feliz programando en Unity.
>
> A pesar de todo, aprendió una valiosa lección: un programador necesita tener unos conocimientos generales que no se aprenden únicamente programando videojuegos.

Aunque parezca un caso hipotético, puedes encontrarte con situaciones similares:

> Pepe ha creado una ruta `/user/rewards` en el servidor que se encarga de dar recompensas a los 30 jugadores con mayor puntuación del torneo, pero tiene que subir los cambios al repositorio y nunca ha usado el comando git a través de un terminal.

> Pepe ha encontrado un bug que no consigue identificar, ya que sólo ocurre cuando hace la build del juego y lo prueba en su móvil.
>
> Podría hacer debugging con `adb logcat -s Unity`, pero Pepe no sabe cómo usar un terminal, así que pierde un día entero haciendo builds a base de prueba y error hasta encontrar la solución sin saber cómo lo ha conseguido.

Ahora que he expuesto varios casos en los que vas a necesitar un terminal, quizás quieras intentarlo por tu cuenta para ahorrarte sorpresas inesperadas.

Si crees que aún no es necesario, no te preocupes. En las próximas páginas tendrás ejemplos más explicativos para que sepas por donde empezar.
