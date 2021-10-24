# Todo es cuestión de abstracción

Cuando empiezas a programar, el lenguaje te ofrece una serie de herramientas para facilitarte la vida. Si necesitas mostrar texto por pantalla, sólo tienes que preocuparte por pasarle el texto que quieres, pero no sabes qué está haciendo el ordenador por debajo para lograr ese objetivo.

A este énfasis en preocuparte únicamente por "¿qué hace?" en lugar de "¿cómo lo hace?" se lo conoce como abstracción.

Cómo ya has podido observar, puedes aprender a programar y trabajar de ello con un lenguaje de programación, pero tendrás muchos, MUCHOS PROBLEMAS.

> Vamos a jugar a un juego:
>
> Te presento una serie de ejercicios escritos en C#. Ya están resueltos,  no quiero que escribas nada ni te pongas a programar.
>
> Antes de cada fragmento de código encontrarás una pregunta; tu objetivo es responderte a ti mismo qué está ocurriendo con sólo leerlo.
>
> Una vez que tengas clara tu respuesta, te recomiendo que investigues para descubrir si estabas en lo cierto.
>
> Si no encuentras la respuesta o sigues teniendo dudas, puedes unirte al Discord de [The Nightmare Community](https://discord.gg/EdtpmDzsDS) para leer la opinión de más programadores que han pasado por esta guía, además de la mía.

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

¿Te han parecido difíciles las preguntas?

Como habrás podido notar, son ejercicios muy simples, pero a su vez tan básicos que no te habrás planteado hasta ahora.

Le damos mucha importancia a saber cuáles son las mejores buenas prácticas de código, ignorando por completo esos pequeños detalles que nos permiten comprender la funcionalidad de un lenguaje y usarlo a nuestro favor.

Nuestro tiempo es muy valioso, y no podemos perderlo con un lenguaje de programación que no sabemos utilizar. De lo contrario, perderás una tarde entera para encontrar la solución a un problema que no entiendes, y le echarás la culpa a ese motor de videojuegos que tanto odiamos, pero al mismo tiempo amamos, porque si nos sacan de ahí, no sabemos programar nada...

La abstracción no lo es todo, mira más allá y encontrarás la respuesta a muchos de tus problemas.