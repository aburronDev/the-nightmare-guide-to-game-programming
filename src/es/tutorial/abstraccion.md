# Todo es cuestión de abstracción

Cuando empiezas a programar, el lenguaje te está ofreciendo una serie de herramientas para facilitarte la vida. Si necesitas mostrar texto por pantalla, sólo tienes que preocuparte por pasarle el texto que quieres, pero no sabes que está haciendo el ordenador por debajo para lograr ese objetivo.

Este énfasis de sólo tener que preocuparte por ¿qué hace? más que en el ¿cómo lo hace? se le conoce como abstracción.

Cómo ya has podido observar, puedes aprender a programar y trabajar de ello con un lenguaje de programación, pero tendrás muchos, MUCHOS PROBLEMAS.

> Vamos a jugar a un juego:
>
> Te presento una serie de ejercicios escritos en C#. Ya están resueltos,  no quiero que escribas nada ni te pongas a programar.
>
> Antes de cada fragmento de código te vas a encontrar una pregunta, y tu objetivo es el de responderte a ti mismo que está ocurriendo con sólo leerlo.
>
> Una vez que tengas claro tu respuesta, te recomiendo que investigues y descubras si estabas en lo cierto.
>
> Si no encuentras la respuesta o sigues teniendo dudas, puedes unirte al discord de [The Nightmare Community](https://discord.gg/EdtpmDzsDS) para leer la opinión de más programadores que han pasado por esta guía, e incluso la mía.

#### ¿El resultado de `score` es `2147483648`?

```csharp
public class Nightmare00
{
	public static void Main()
	{
		int score = 2147483647;

		score++;
	}
}
```

#### ¿Con qué valor se inicializa `c`?

```csharp
public class Nightmare01
{
	public static void Main()
	{
		char c = System.Convert.ToChar(48);
	}
}
```

#### ¿Este programa compila?

```csharp
public class Nightmare02
{
	public static void Main()
	{
		while(true);
	}
}
```

#### ¿Cuál es el valor de `life` después de llamar al método `Damage`?
```csharp
public class Nightmare03
{
	public static void Damage(int life, int amount)
	{
		life -= amount;
	}

	public static void Main()
	{
		int life = 100;

		System.Console.WriteLine($"Initial life = {life}");
		Damage(life, 25);
		System.Console.WriteLine($"Current life = {life}");
	}
}
```

#### ¿Por qué puedo acceder al valor de un índice en `gameState` si no está declarado como `string[]`?
```csharp
public class Nightmare04
{
	public static void Main()
	{
		string gameState = "Game Over";

		System.Console.WriteLine($"gameState[0] = {gameState[0]}");
	}
}
```

#### ¿Por qué el valor de `pCurrentWave` nunca es el mismo?
```csharp
public class Nightmare05
{
	public static void Main()
	{
		unsafe
		{
			int currentWave = 42;
			int* pCurrentWave = &currentWave;

			System.Console.WriteLine($"pCurrentWave = {(int)pCurrentWave}");
		}
	}
}
```

¿Te han parecido díficiles las preguntas?

Como has podido notar, son ejercicios muy simples, pero a su vez son tan básicos que no te habrás replanteado hasta ahora.

Le damos mucha importancia a las mejores prácticas de código, cuando ni siquiera le prestamos atención a esos pequeños detalles que nos permiten comprender la funcionalidad de un lenguaje, y poder usarlo a nuestro favor.

Nuestro tiempo es muy valioso, y no podemos perderlo con un lenguaje de programación que no sabemos utilizar. De lo contrario, perderás una tarde entera para encontrar la solución a un problema que no entiendes, y le echarás la culpa a ese motor de videojuegos que tanto odiamos pero al mismo tiempo amamos, porque si nos sacan de ahí no sabemos programar...

La abstracción no lo es todo, mira más allá y encontrarás la respuesta a muchos de tus problemas.