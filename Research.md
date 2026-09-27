# Paradigma Challenge
- Merlijn Cremers
- 2119805
- versie 0.1
- 27/09/2026
- Dennis Breuker
- APP




## Inleiding-01

Voor het controleren van de spelling is gebruik gemaakt van ChatGPT (OpenAI, 2026).

## Research-02

> "Object-oriented programming an exceptionally bad idea which could only have originated in California" - Dijkstra


Elixir is een functionele programmeertaal met een aantal interessante eigenschappen en concepten. **Immutability** en **recursion** zijn een groot deel van de taal, net als **pure functies**.
Het meest interessante voor mij was toch wel de stijl van schrijven. Kort samengevat gaat het vooral om **wat er moet gebeuren**, in plaats van stap voor stap te beschrijven **hoe** het moet gebeuren.

### Functions
Functies schrijf je net wat anders in elixir, je gebuikt geen haakjes maar `do` en `end`
```
defmodule Greeter do
def hello(name) do
"Hello, " <> name
end
end

Greeter.hello("world")
```

Ook zijn er **anonieme functies** met `fn`

```
code voorbeeld komt nog
```

Oftewel functies zonder naam.

### Pattern Matching

### Pipe Operator
 Zo is er ook de interessante `|>` pipe-functie 
 
Een voorbeeld van elixirschool.com
```
"Elixir rocks" |> String.upcase() |> String.split()
["ELIXIR", "ROCKS"]
```
Hiermee geef je de ene functie direct als input aan de volgende.

### Recursion
Recursie gaat 100% een belangrijk deel zijn van deze challenge, ik heb namelijk geen for of while loops, dus recursie moet voor mij de for loop worden.
In elixir is de stop conditie **do: 0**


Voorbeeld van elixir examples.com
```
defmodule MyList do
  # Base case: an empty list has length 0
  def length([]), do: 0

  # Recursive case: the length is 1 + the length of the tail
  def length([_head | tail]), do: 1 + length(tail)
end
```

Of (snel even zelf geschreven),

```
def countdown(0) do
  IO.puts("Klaar denk ik wel")
end

def countdown(n) do
  IO.puts(n)
  countdown(n - 1)
end

```
### Booleans

Booleans zijn ook een tikje anders. Het zijn namelijk eigenlijk waarden van het datatype **atom**. De waarde van een atom is zijn naam, bijvoorbeeld `:true` of `:false`.

Bij booleans heb je ook de operators `and`, `or` en `not`. Deze werken vergelijkbaar met `&&` of `||`, maar lezen wat makkelijker.

Atoms worden verder nog door Elixir heen gebruikt voor andere waarden of plekken, maar die zijn momenteel niet relevant.

## Challenge-03

## Implementatie-04

## Conclusie-05

## Bronnen-06

- [Elixir School](https://elixirschool.com/en) — 18/09/2026
- [Elixir HexDocs](https://elixir.hexdocs.pm/) — 18/09/2026