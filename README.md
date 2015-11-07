# Een webpagina maken - HTML - Les 1

## Overzicht

Vandaag gaan we [HTML](http://nl.wikipedia.org/wiki/HTML) gebruiken. We gaan in een webbrowser een verhaal vertellen dat we aan onze vrienden en familie kunnen laten zien.

```html
<p>HTML een opmaaktaal die we kunnen gebruiken om structuur en vorm te geven aan ons verhaal in een webbrowser. Chrome, Safari, Firefox en Internet Explorer zijn voorbeelden van webbrowsers. Als we HTML gebruiken om een verhaal in de browser te vertellen, maken we een webpagina.</p>
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

![demo](http://cl.ly/image/0e1d3b2C3y2P/content#.png)

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

Now tell more of your story, what else happened?

```html
<html>
  <head>
  </head>
  <body>
    Today I took the dogs to the park and we had a great time!

    After the dogs played with their friends we took a walk around the track together.
  </body>
</html>
```

![Telling more of the story](http://cl.ly/image/2w1Q090V1b2t/content#.png)

## Using Paragraphs

Here you can see that I separated my paragraphs using new lines (on the right) but the rendered html (on the left) didn't get separated into paragraphs. This is because I did not use HTML to add  paragraph (`<p>` tags) to my story.

Add the `<p>` around the paragraphs:

```html
<html>
  <head>
  </head>
  <body>
    <p>Today I took the dogs to the park and we had a great time!</p>
    <p>After the dogs played with their friends we took a walk around the track together.</p>
  </body>
</html>
```

![Adding paragraph tags](http://cl.ly/image/1U053V060k0u/content#.png)

Now the paragraphs are displayed correctly!

## Adding a Title

Next add a title to your story. To do this add the `<title>` to the `<head>` and then add it to the `<body>` using `<h1>` tags.

```html
<html>
  <head>
    <title>A day at the dog park</title>
  </head>
  <body>
    <h1>A day at the dog park</h1>
    <p>Today I took the dogs to the park and we had a great time!</p>
    <p>After the dogs played with their friends we took a walk around the track together.</p>
  </body>
</html>
```

![Story with title](http://cl.ly/image/1e352r043A1x/content#.png)

## Picture Time!

This story would be a lot more interesting with pictures! Adding a picture to our story is simple, we just use the `<img>` tag and tell it where our image is.

The `<img>` tag has an attribute called `src` and this is where we tell it the url to the image we want to use in our story. Here is an example `<img>` tag:

```html
<img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
```

Adding this to our story is easy:

```html
<html>
	<head>
		<title>A day at the dog park</title>
	</head>
	<body>
		<h1>A day at the dog park</h1>
		<p>Today I took the dogs to the park and we had a great time!</p>
		<img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
		<p>After the dogs played with their friends we took a walk around the track together.</p>
		<img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
	</body>
</html>
```


![Story with images](http://cl.ly/image/3w2d1C0P1N3I/content#.png)

## Strong and Emphasis

Sometimes we want to bring more attention to parts of our story. One way we can do this is by using the `<strong>` tag to make certain parts of our story look bolder compared to other parts. Here is an example:

```html
<html>
  <head>
    <title>A day at the dog park</title>
  </head>
  <body>
    <h1>A day at the dog park</h1>
    <p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>After the dogs played with their friends we took a walk around the track together.</p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
  </body>
</html>
```

![Story with strong](http://cl.ly/image/1u083V0I0Y3O/content#.png)

We can bring emphasis to parts of our story by *making them italic*. We use the `<em>` tag for emphasis. Here is an example:

```html
<html>
  <head>
    <title>A day at the dog park</title>
  </head>
  <body>
    <h1>A day at the dog park</h1>
    <p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>After the dogs played with their friends <em>we took a walk around the track together.</em></p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
  </body>
</html>
```

![Story with emphasis](http://cl.ly/image/45033t3W3v3R/content#.png)

## Lists

You can easily add a list to your story using `<ul>` and `<li>` tags. Here is an example:

```html
<html>
	<head>
		<title>A day at the dog park</title>
	</head>
	<body>
		<h1>A day at the dog park</h1>
		<p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>After the dogs played with their friends <em>we took a walk around the track together.</em></p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
		<p>While we were at the dog park we saw many kinds of dogs, including:</p>
		<ul>
			<li>Poodles</li>
			<li>Great Danes</li>
			<li>Black Labs</li>
		</li>
	</body>
</html>
```

The `<ul>` tag tells the browser this is a list of items. The `<li>` tags are used around each list item.

![Story with list of dogs](http://cl.ly/image/3E2k0C3k3u3N/content#.png)

If you want the list to use numbers instead of bullet points you can change the `<ul>` tag (unordered list) to an `<ol>` tag (ordered list).

```html
<html>
	<head>
		<title>A day at the dog park</title>
	</head>
	<body>
		<h1>A day at the dog park</h1>
		<p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>After the dogs played with their friends <em>we took a walk around the track together.</em></p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
		<p>While we were at the dog park we saw many kinds of dogs, including:</p>
		<ol>
			<li>Poodles</li>
			<li>Great Danes</li>
			<li>Black Labs</li>
		</ol>
	</body>
</html>
```

![Story with ordered list](http://cl.ly/image/3x2t1c1N1v3o/content#.png)

## Hyperlinks

One of the things that makes web pages so amazing for telling stories is you can **link** things together with other web pages on the internet and it is really easy to do!

In the pervious example I included three kinds of dogs that we saw at the park, now I'm going to use hyperlinks (the `<a>` tag) to link the dog names to their descriptions on Wikipedia.

The `<a>` tag has an attribute called `href` and we will set that attribute equal to the url of the web page we want to link to. Here is an example where I link the word Poodles to the web page about Poodles on Wikipedia:

```
<a href="http://en.wikipedia.org/wiki/Poodle">Poodles</a>
```

Here is what it looks like in the context of our story:

```html
<html>
	<head>
		<title>A day at the dog park</title>
	</head>
	<body>
		<h1>A day at the dog park</h1>
		<p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>After the dogs played with their friends <em>we took a walk around the track together.</em></p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
		<p>While we were at the dog park we saw many kinds of dogs, including:</p>
		<ul>
			<li><a href="http://en.wikipedia.org/wiki/Poodle">Poodles</a></li>
			<li><a href="http://en.wikipedia.org/wiki/Great_Dane">Great Danes</a></li>
			<li><a href="http://en.wikipedia.org/wiki/Labrador_Retriever">Black Labs</a></li>
		</li>
	</body>
</html>
```

## Telling More Than One Story

If you want to write another story you don't have to start a whole new web page, you can use the same page you have been working on and use HTML to indicate where one story stops and the next begins. Typically we will use `<article>` tags to accomplish this. Here is an example:

```html
<html>
  <head>
    <title>A day at the dog park</title>
  </head>
  <body>
    <h1>Dog Stories</h1>
    <article>
      <h2>A day at the dog park</h2>
      <p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
      <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
      <p>After the dogs played with their friends <em>we took a walk around the track together.</em></p>
      <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
      <p>While we were at the dog park we saw many kinds of dogs, including:</p>
      <ul>
        <li><a href="http://en.wikipedia.org/wiki/Poodle">Poodles</a></li>
        <li><a href="http://en.wikipedia.org/wiki/Great_Dane">Great Danes</a></li>
        <li><a href="http://en.wikipedia.org/wiki/Labrador_Retriever">Black Labs</a></li>
      </li>
    </article>
    <article>
      <h2>Driving Across The Country With Leo and Bailey</h2>
      <p>A year ago we drove across the country <em>with Leo and Bailey</em> when we moved from Indiana to California.</p>
      <img src="http://cl.ly/image/3G2Z3x0G3Z46/content#.png">
      <p>One time after stopping to eat lunch we found Leo in the front seat ready to drive. <strong>This made us laugh really hard :)</strong></p>
    </article>
  </body>
</html>
```

You will notice a few new things in the html above. We added a second story, we enclosed both stories in `<article>` tags, we changed the story titles to use `<h2>` (Heading 2) tags, and we changed the `<h1>` (Heading 1) at the top to say **Dog Stories**.

## Style

In the next lesson we will start learning how to add style to our story using html attributes and css. Here is an example to help get you excited about the next lesson.

In Codepen we want to check the box next to CSS and then paste the following css code into the CSS box:

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

![Story with CSS](http://cl.ly/image/002B0l3l090P/content#.png)

## Advanced Topics

### HTML Doctype

Web browsers look for a document type tag at the beginning of an HTML document in order to determine how they should read and render the HTML. We can add the `<!DOCTYPE html>` tag to our web page to tell browsers that we are using the latest version of HTML.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>A day at the dog park</title>
  </head>
  <body>
    <h1>A day at the dog park</h1>
    <p>Today I took the dogs to the park and <strong>we had a great time!</strong></p>
    <img src="http://f.cl.ly/items/2f473l1d233S0S1k3J3d/dogs-playing.jpg">
    <p>After the dogs played with their friends <em>we took a walk around the track together.</em></p>
    <img src="http://f.cl.ly/items/0o0T0V0g261C1R0I022z/walking-the-track.jpg">
    <p>While we were at the dog park we saw many kinds of dogs, including:</p>
    <ul>
      <li>Poodles</li>
      <li>Great Danes</li>
      <li>Black Labs</li>
    </ul>
  </body>
</html>
```
You can read more about document type [here](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5/Introduction_to_HTML5).

## Other Resources

* [HTML Glossary](http://www.codecademy.com/glossary/html)
* [Mozilla Developer Network](https://developer.mozilla.org/en-US/)
