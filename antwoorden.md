# Theoretische vragen

## Opdracht 1
Wat doen de functies `int(x)`, `float(x)`, `str(x)`?

Die retourneren x als integer (geheel getal), floating point number (komma getal) of als string.
Bijvoorbeeld, `int("123")` maakt van de string `"123"` de integer `123`.
Als dit niet lukt, dan gooit de functie een uitzondering (exception).
Bijvoorbeeld, `float("x8nw")` zal niet werken, want de inhoud van de string `"x8nw"` is geen komma getal.

## Opdracht 2
Welk van de volgende statements kun je gebruiken om 1 bij het getal x op te tellen? (Er kunnen meerdere antwoorden goed zijn)
- `x = x + 1`
- `x += 1`

## Opdracht 3
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

## Opdracht 4
Welk van de volgende identifiers is niet een legale naam voor een variable in python?
- `my-variable`. Dit is omdat het kleine streepje (`-`) gebruikt wordt als min teken. Je mag die dus niet in de naam van een variable doen.

# Opdracht 5
Welk van de volgende operators kun je gebruiken om de rest van een deelsom uit te rekenen?
- `%`

## Opdracht 6
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

## Opdracht 7
Wat is de output van deze code?
```py
a = 10
b = 5
c = 3
d = a + b * c
print(d)
```
- `25`

## Opdracht 8