# Theoretische vragen

## Opdracht 1.1
Wat doen de functies `int(x)`, `float(x)`, `str(x)`?

Die retourneren x als integer (geheel getal), floating point number (komma getal) of als string.
Bijvoorbeeld, `int("123")` maakt van de string `"123"` de integer `123`.
Als dit niet lukt, dan gooit de functie een uitzondering (exception).
Bijvoorbeeld, `float("x8nw")` zal niet werken, want de inhoud van de string `"x8nw"` is geen komma getal.

## Opdracht 1.2
Welk van de volgende statements kun je gebruiken om 1 bij het getal x op te tellen? (Er kunnen meerdere antwoorden goed zijn)
- `x = x + 1`
- `x += 1`

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
### `foo(5)`
`5` is niet minder dan `0`, dus de eerste `if`-statement gaat niet af.
Omdat de eerste if-statement niet af gaat, kijken we nu naar de `elif`-statement. Deze gaat alleen af als de voorafgaande `if` niet afgaat.
`5` is wel minder dan `10`, dus er wordt hier `5` geprint.
De laatste `if`-statement staat los van de 2 `if`-statements erboven, want er staat geen `else` voor. We moeten dus deze branch checken.
`5` is niet meer dan `5`, dus deze `if`-statement gaat niet af.
Output:
```
5
```
### `foo(-3)`
`-3` is wel minder dan `0`, dus de eerste `if`-statement gaat af, en `-3` wordt geprint. Omdat de eerste `if`-statement af gaat, wordt de `elif`-statement niet gecheckt. Dat betekent dat deze sowieso niet af gaat.
`-3` is niet meer dan `5`, dus de laatste `if`-statement gaat ook niet af.
Output:
```
-3
```
### `foo(7)`
`7` is niet minder dan `0`, dus de eerste `if`-statement gaat niet af.
Omdat de eerste if-statement niet af gaat, kijken we nu naar de `elif`-statement. Deze gaat alleen af als de voorafgaande `if` niet afgaat.
`7` is wel minder dan `10`, dus er wordt hier `7` geprint.
De laatste `if`-statement staat los van de 2 `if`-statements erboven, want er staat geen `else` voor. We moeten dus deze branch checken.
`7` is wel meer dan `5`, dus ook deze `if`-statement gaat af. `7` wordt dus nog een keer geprint.
Output:
```
7
7
```

## Opdracht 1.4
Welk van de volgende identifiers is niet een legale naam voor een variable in python?
- `my-variable`. Dit is omdat het kleine streepje (`-`) gebruikt wordt als min teken. Je mag die dus niet in de naam van een variable doen.

## Opdracht 1.5
Welk van de volgende operators kun je gebruiken om de rest van een deelsom uit te rekenen?
- `%`

## Opdracht 1.6
Bekijk het volgende stukje code
```py
def bar(a, b):
    if (a <= b):
        return b
    else:
        return a
```
Leg in je eigen woorden uit wat `bar(1, 2)` en `bar(4, 3)` returnen. Wat doet de functie `bar`?

### `bar(1, 2)`
In dit geval hebben we `a == 1` en `b == 2`. `a` is minder of gelijk aan `b`, dus retourneert de functie `b`. Dat is `2`.
### `bar(4, 3)`
In dit geval hebben we `a == 4` en `b == 3`. `a` is niet minder of gelijk aan `b`, dus retourneert de functie `a` via de `else`. Dat is `4`.\
Deze functie retourneert altijd de grootste van de twee inputwaardes.

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

## Opdracht 1.9
Welke van de volgende statement(s) kan je gebruiken als een conditie in bijvoorbeeld een `if`-statement?
- `x == x`

## Opdracht 1.10
In welk van de volgende gevallen is `x` altijd `True`?
- `x = not False`
- `x = (7 == 7)`

# Programmeer vragen
Dit is zijn allemaal voorbeelden, er zijn meerdere antwoorden goed.

## Opdracht 2.1
Schrijf een functie die als input de lengte en de breedte van een rechthoek neemt, en de oppervlakte van deze rechthoek retourneert.\

```py
def calculate_rectangle_area(lengte, breedte):
    return lengte * breedte
```

## Opdracht 2.2
Schrijf een functie die als input een geheel getal neemt, en `True` retourneert als het getal even is, en `False` retourneert als het getal oneven is.
```py
def is_even(getal):
    if (getal % 2 == 0):
        return True
    else
        return False
```

## Opdracht 2.3
Om het aantal woorden in een zin te tellen kun je alle spaties in de zin tellen. Bijvoorbeeld, de zin `"Vandaag is het lekker weer.` heeft 4 spaties.\
Schrijf een functie die op deze manier het aantal woorden in een `string` telt. Je mag ervan uitgaan dat er geen extra onnodige spaties voor of na de zin staan.
```py
def word_count(zin):
    count = 1
    for letter in zin:
        if (letter == ' '):
            count += 1
    return count
```