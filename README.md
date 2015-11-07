# Een webpagina maken - HTML - Les 1

## Overzicht

Vandaag gaan we [HTML](http://nl.wikipedia.org/wiki/HTML) gebruiken. We gaan in een webbrowser een verhaal vertellen dat we aan onze vrienden en familie kunnen laten zien.

```html
<p>
HTML een opmaaktaal die we kunnen gebruiken om structuur en vorm te geven aan ons verhaal in een webbrowser. 
Chrome, Safari, Firefox en Internet Explorer zijn voorbeelden van webbrowsers. 
Als we HTML gebruiken om een verhaal in de browser te vertellen, maken we een webpagina.
</p>
```

Een webpagina bestaat uit een heleboel HTML elementen. Elk element noemen we een "tag". De tekst hierboven is een voorbeeld van hoe je een paragraaf maakt in HTML, door er de tag `<p>` omheen te zetten.

**Omschrijving**

Om te starten met onze webppagina moeten we leren hoe we HTML moeten gebruiken. Vandaag gaan we:

* Beginnen met een basis HTML voorbeeld
* Een verhaal vertellen en HTML toepassen om de structuur en vorm toe te voegen

**Demo**

Dit stukje HTML:

```
<!DOCTYPE html>
<html>
  <head>
    <title>Mijn dag op werk</title>
  </head>
  <body>
    <h1>Mijn dag op werk</h1>
    <p>Ik heb op werk een leuke dag vandaag. Ik heb mijn taken afgerond en een collega geholpen.</p>
    <p>Mijn taken waren:</p>
    <ul>
      <li>Een <strong>vind ik leuk</strong> functie toevoegen</li>
      <li>Deze testen in de testomgeving</li>
      <li>Daarna deze ook in de productieomgeving uit zetten</li>
      <li>Een blog schrijven over het maken van de <strong>vind ik leuk</strong> functie</li>
    </ul>
    <p>Vandaag was een hele leuke dag!</p>
  </body>
</html>
```

Dit maakt een webppagina die er ongeveer zo uit ziet:

![demo](http://cl.ly/image/112F1O2b3t3a)

Hier kun je een [demo](http://codepen.io/anon/pen/gaBMjV?editors=100) vinden om zelf te experimenteren.

## Wat hebben we nodig

**Gereedschap**

* [CODEPEN](http://codepen.io/pen/)

## Om te beginnen

Om te beginnen starten we een blanco project op CODEPEN:
[http://codepen.io/pen/](http://codepen.io/pen/?editors=100)

![CODEPEN blanco project](http://cl.ly/image/35081n120I42/content#.png)

Nu voegen we de minimale HTML toe om een werkende webpagina te maken. Start door in het HTML gebied te klikken en voeg dan de `<html>` tag toe, openen en sluiten.

```html
<html>
</html>
```

Je scherm zou er nu zo uit moeten zien:

![CODEPEN na toevoegen HTML tags](http://cl.ly/image/1y1H1M1n2r1m/content#.png)

Daarna voegen we de `<head>` en `<body>` tags toe. De `<body>` tags is het stukje dat de webbrowser verteld wat er weergegeven moet worden. Onze HTML ziet er nu zo uit:

```html
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```

## Je verhaal vertellen

Je kunt nu beginnen met je verhaal te vertellen door binnen de `<body` tag iets neer te zetten. Bijvoorbeeld:

```html
<html>
  <head>
  </head>
  <body>
    Vandaag zijn we met de honden naar het park geweest. We hebben veel plezier gehad!
  </body>
</html>
```

![Basis demo van HTML](http://cl.ly/image/2P3l3V1A302i/content#.png)

Nu gaan we meer van ons verhaal vertellen. Wat is er gebeurd?

```html
<html>
  <head>
  </head>
  <body>
    Vandaag zijn we met de honden naar het park geweest. We hebben veel plezier gehad!

    Nadat de honden met hun vriendjes hebben gespeeld zijn we verder gaan wandelen.
  </body>
</html>
```

![Meer van het verhaal](http://cl.ly/image/2w1Q090V1b2t/content#.png)

## Een paragraaf toevoegen

Om een paragraaf toe te voegen in HTML gebruikn je de `<p>` tag. Vergeet niet om de tag ook te sluiten!

Zoals je ziet heeft de HTML Weergave niet begrepen dat de tekst op verschillende regels getoond moet worden. Dit komt omdat ik dat niet heb verteld, want in mijn HTML stonden geen `<p>` tags in het verhaal. 

Voeg de tag `<p>` toe aan elke regel:

```html
<html>
  <head>
  </head>
  <body>
    <p>Vandaag zijn we met de honden naar het park geweest. We hebben veel plezier gehad!</p>
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we verder gaan wandelen.</p>
  </body>
</html>
```

![Adding paragraph tags](http://cl.ly/image/1U053V060k0u/content#.png)

Nu worden de regels wel goed getoond!

## Een titel toevoegen

Nu gaan we een titel toevoegen aan het verhaal. Dit doen we op twee plaatsen: in een `<title>` tag binnen de `<head>` (zodat de browser weet hoe deze pagina heet) en in de `<body>` met een `<h1>` tag.

h1 staat voor "Heading 1" oftewel "Kop 1".

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. We hebben veel plezier gehad!</p>
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we verder gaan wandelen.</p>
  </body>
</html>
```

![Verhaal met titel](http://cl.ly/image/1e352r043A1x/content#.png)

## Tijd voor plaatjes!

Dit verhaal wordt een stuk leuker om te lezen als er ook plaatjes bij staan! Om de browser te vertellen dat er een plaatje getoond moet worden gebruiken we de `<img>` tag. 

De `<img>` tag heeft een attribuut (of een eigenschap) die `src` heet. Dit geeft door aan de browser waar de afbeelding vandaan moet komen die we in ons verhaal willen gebruiken. Hier is een voorbeeld van een `<img>` tag:

```html
<img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
```

En zo voegen we het plaatje toe aan ons verhaal:

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. We hebben veel plezier gehad!</p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we verder gaan wandelen.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
  </body>
</html>
```


![Verhaal met plaatjes](http://cl.ly/image/3w2d1C0P1N3I/content#.png)

## Vet en cursief

Soms willen we een bepaald stukje in ons verhaal er meer uit laten springen. Dit kunnen we doen door een stukje tekst vet te maken, zodat het er dikker uit ziet dan de rest van de tekst. Dit doen we met de `<strong>` tag. Strong is engels voor 'sterk'. Hier een een voorbeeld:

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. <strong>We hebben veel plezier gehad!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we verder gaan wandelen.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
  </body>
</html>
```

![Verhaal met vetgedrukt](http://cl.ly/image/1u083V0I0Y3O/content#.png)

We kunnen ook meer nadruk geven op een deel van ons verhaal door een stuk *tekst cursief te maken*. Hiervoor gebruiken we de tag `<em>`. Dit staat voor emphasis, wat engels is voor "nadruk". Hier is een voorbeeld:

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. <strong>We hebben veel plezier gehad!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we <em>verder gaan wandelen</em>.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
  </body>
</html>
```

![Verhaal met nadruk](http://cl.ly/image/45033t3W3v3R/content#.png)

## Lijsten en opsommingen

Voor het toevoegen van lijsten of opsommingen kun je de `<ul>` of `<ol>` tags gebruiken. ul staat voor Unnumbered List, engels voor ongenummerde lijst. ol staat voor Ordered List, engels voor genummerde lijst. Je geeft vervolgens met de `<li>` tag aan dat iets een onderdeel is van die lijst. Hier is een voorbeeld:

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. <strong>We hebben veel plezier gehad!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we <em>verder gaan wandelen</em>.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
    <p>In het park hebben we veel andere honden gezien, bijvoorbeeld:</p>
    <ul>
      <li>Herdershond</li>
      <li>Labrador</li>
      <li>Dalmatier</li>
    </ul>
  </body>
</html>
```

De `<ul>` tag verteld de browser dat dit een lijst met dingen is. De `<li>` tags geeft aan dat iets een onderdeel is van die lijst.

![Verhaal met een lijst met honden](http://cl.ly/image/3E2k0C3k3u3N/content#.png)

Als je de lijst wilt laten tellen met getallen in plaats van de punten, verander je de `<ul>` tag in een `<ol>` tag. De browser geeft dan zelf nummers aan de lijst.

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. <strong>We hebben veel plezier gehad!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we <em>verder gaan wandelen</em>.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
    <p>In het park hebben we veel andere honden gezien, bijvoorbeeld:</p>
    <ol>
      <li>Herdershond</li>
      <li>Labrador</li>
      <li>Dalmatiër</li>
    </ol>
  </body>
</html>
```

![Verhaal met genummerde lijst](http://cl.ly/image/3x2t1c1N1v3o/content#.png)

## Hyperlinks

Een hyperlink, of link, geeft aan de browser aan dat een woord doorgekoppeld wordt naar een andere pagina op het internet. Hiermee kun je heel makkelijk extra informatie of verwijzingen toevoegen aan je verhaal. En het is heel makkelijk te doen!

In het vorige voorbeeld hebben we drie verschillende honden genoemd die we in het park hebben gezien. Nu gaan we met hyperlinks (de `<a>` tag) een koppeling maken naar deze honden op Wikipedia.

De `<a>` tag heeft een attribuut `href`. In dit attribuut vertellen we waar de andere webpagina staat waar we naar toe willen linken. Voor de Wikipedia pagina over de Herdershons is dat bijvoorbeeld:

```
<a href="https://nl.wikipedia.org/wiki/Herdershond">Herdershond</a>
```

En zo komt dat er dan uit te zien in ons verhaal:

```html
<html>
  <head>
    <title>Op stap met de honden</title>
  </head>
  <body>
    <h1>Op stap met de honden</h1>
    <p>Vandaag zijn we met de honden naar het park geweest. <strong>We hebben veel plezier gehad!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we <em>verder gaan wandelen</em>.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
    <p>In het park hebben we veel andere honden gezien, bijvoorbeeld:</p>
    <ul>
      <li><a href="https://nl.wikipedia.org/wiki/Herdershond">Herdershond</a></li>
      <li><a href="https://nl.wikipedia.org/wiki/Labrador_retriever">Labrador</a></li>
      <li><a href="https://nl.wikipedia.org/wiki/Dalmatier">Dalmatiër</a></li>
    </ul>
  </body>
</html>
```

## Meer verhalen vertellen

Als je nog een verhaal wilt vertellen, kun je een nieuwe webpagina maken. Je kunt ook binnen dezelfde webpagina een nieuw verhaal vertellen. In HTML geeft je dan aan waar het verhaal start en stopt, en waar de volgende begint. Dit kun je doen door de `<article>` tag te gebruiken. Hier is een voorbeeld:

```html
<html>
  <head>
    <title>Hondenverhalen</title>
  </head>
  <body>
    <h1>Hondenverhalen><h1>
    <article>
      <h2>Op stap met de honden</h2>
      <p>Vandaag zijn we met de honden naar het park geweest. <strong>We hebben veel plezier gehad!</strong></p>
      <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
      <p>Nadat de honden met hun vriendjes hebben gespeeld zijn we <em>verder gaan wandelen</em>.</p>
      <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
      <p>In het park hebben we veel andere honden gezien, bijvoorbeeld:</p>
      <ul>
        <li><a href="https://nl.wikipedia.org/wiki/Herdershond">Herdershond</a></li>
        <li><a href="https://nl.wikipedia.org/wiki/Labrador_retriever">Labrador</a></li>
        <li><a href="https://nl.wikipedia.org/wiki/Dalmatier">Dalmatiër</a></li>
      </ul>
    </article>
    <article>
      <h2>In de auto</h2>
      <p>We hebben de honden in de auto meegenomen. We zijn even gestopt om een boterham te eten.</p>
      <img src="http://cl.ly/image/3G2Z3x0G3Z46/content#.png">
      <p>Toen we weer verder wouden is Leo achter het stuur gaan zitten. <strong>Wat een grappige hond is het toch!</strong></p>
    </article>
  </body>
</html>
```

Zoals je kunt zien zijn er een paar dingen veranderd in de HTML. We hebben een tweede verhaal toegevoegd. Beide verhalen zijn nu binnen een `<article>` tag gezet. Ook hebben we de titel van de pagina veranderd in **Hondenverhalen** en bij elk verhaal een kleiner kopje gebruikt, namelijk een `<h2>` oftewel Kop 2.

## Stijlen, kleuren en meer

De volgende keer gaan we leren hoe we de stijl en kleur van onze HTML kunnen aanpassen. Dit doen we door gebruik te maken van CSS. Hier is vast een voorproefje:

Zet het vakje CSS aan in Codepen, en vul dit in het CSS vakje in:

```css
body {
  font-family: Arial;
  background-color: #eee;
  color: green;
}

img {
  border: 2px solid green;
  padding: 2px;
}
```

![Verhaal met CSS](http://cl.ly/image/002B0l3l090P/content#.png)
