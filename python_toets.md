# Theoretische vragen

## Opdracht 1.1
Wat doen de functies `int(x)`, `float(x)`, `str(x)`?

## Opdracht 1.2
Welk van de volgende statements kun je gebruiken om 1 bij het getal x op te tellen? (Er kunnen meerdere antwoorden goed zijn)
- `x = x + 1`
- `x == x + 1`
- `x += 1`
- `x + 1 = x`

## Opdracht 1.3
Bekijk het volgende stukje code
```py
def foo(x):
    if (x < 0):
        print(x)
    elif (x < 10):
        print(x)
    if (x > 5):
        print(x)
```
Leg uit wat de volgende statements printen:
- `foo(5)`
- `foo(-3)`
- `foo(7)`

## Opdracht 1.4
Welk van de volgende identifiers is niet een legale naam voor een variable in python?
- `my-variable`
- `my_variable`
- `MyVariable`
- `myVariable`

## Opdracht 1.5
Welk van de volgende operators kun je gebruiken om de rest van een deelsom uit te rekenen? (`97` gedeeld door `10` heeft rest `7`)
- `/`
- `%`
- `**`
- `//`

## Opdracht 1.6
Bekijk het volgende stukje code
```py
def bar(a, b):
    if (a <= b):
        return b
    else:
        return a
```
Leg in je eigen woorden uit wat `bar(1, 2)` en `bar(4, 3)` returnen. Wat doet de functie bar?

## Opdracht 1.7
Wat is de output van deze code?
```py
a = 10
b = 5
c = 3
d = a + b * c
print(d)
```
- `25`
- `45`
- `18`
- `d`

## Opdracht 1.8
Wat is de output van deze code?
```py
a = 10
b = a * 2
c = a + 1
d = a + b + c
print(d)
```
- `41`
- `51`
- `abc`
- `31`

## Opdracht 1.9
Welke van de volgende statement(s) kan je gebruiken als een conditie in bijvoorbeeld een `if`-statement?
- `x = 2`
- `a * b = 3`
- `x => b + 3`
- `x == x`

## Opdracht 1.10
In welk van de volgende gevallen is `x` altijd `True`?
- `x = x * True`
- `x = not False`
- `x = (7 == 7)`
- `x = x`

# Programmeer vragen
Maak bij al deze vragen gebruik van een net formaat en geef elke functie of variable een passende naam.

## Opdracht 2.1
Schrijf een functie die als input de lengte en de breedte van een rechthoek neemt, en de oppervlakte van deze rechthoek retourneert.

## Opdracht 2.2
Schrijf een functie die als input een geheel getal neemt, en `True` retourneert als het getal even is, en `False` retourneert als het getal oneven is.

## Opdracht 2.3
Om het aantal woorden in een zin te tellen kun je alle spaties in de zin tellen. Bijvoorbeeld, de zin `"Vandaag is het lekker weer.` heeft 4 spaties.\
Schrijf een functie die op deze manier het aantal woorden in een `string` telt. Je mag ervan uitgaan dat er geen extra onnodige spaties voor of na de zin staan.