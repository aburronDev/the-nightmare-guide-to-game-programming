# A matter of abstraction

When starting in programming, the language is offering you a set of tools to make your life easier. If you need to display text on the screen, just type and forget. However, you might not know what the computer is doing underneath the code.

Focusing on "what it does” rather than “how is doing it” is called “abstraction”.

As you have seen, you can learn to program and work at it with a programming language, but you will encounter many, MANY PROBLEMS.

>Let's play a game
>
>I present you a series of exercises written in C#. They are already solved, I don't want you to write anything or get into programming yet.
>
>Before each code fragment you’ll find a question, and your goal is to answer yourself what is happening just by reading it.
>
>Once you are sure about your answer, I recommend you do some research and find out if you were right.
>
>If you don't find the answer or you still have doubts, you can join [The Nightmare Community](https://discord.gg/EdtpmDzsDS) discord to read the opinion of more programmers who have gone through this guide, and even mine.

#### Is the `score` result `2147483648`?

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

#### With which value does `c` initialize?

```csharp
public class Nightmare01
{
	public static void Main()
	{
		char c = System.Convert.ToChar(48);
	}
}
```

#### Does this program compile?

```csharp
public class Nightmare02
{
	public static void Main()
	{
		while(true);
	}
}
```

#### What is the `life` value after calling the `Damage` method?

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

#### Why can I access an index value in `gameState` if it’s not declared as `string[]`?
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

#### Why is `pCurrentWave` value never the same?
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
Did you find it difficult?

As you may have noticed, these are very simple exercises, so basic in fact that you may not have thought about them until now.

We give so much importance to the best coding practices that we don't pay attention to those little details that allow us to understand the functionality of a language, and use it to our advantage.

Our time is valuable, and we cannot afford wasting it with a programming language that we don’t know how to use. Otherwise, you’ll find yourself wasting a whole afternoon to find the solution to a problem you don't understand, and you’ll probably blame that game engine we hate but at the same time we love so much, because if they take us out of there and think outside the box, we don't know how to program...

Abstraction is not everything, look beyond and you’ll find the answer to many problems.
