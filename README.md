# Tutorial

Tutorial html

<section>sekcja</section>
<p>akapit</p>
<a>link</a>
<button>przycisk</button>
<h1>Nagłówek</h1>
<!-- Komentarz -->
Odnośniki http >
<p> Tytuł linku <a href="link" target="_blank" (otwiera nową kartę w przeglądarce) rel="noopener noreferrer"(antimalware) >nazwa linku</a>.</p>
target="_self" > domyślny target linku (otwiera się na aktualnie wyświetlanej stronie)
<img src="link" /> <> fotka
lista nieuporządkowana (punktowa)
<ul> 
  <li><a>pozycja1</a></li>
  <li>pozycja2</li>
</ul>
Lista uporządkowana (numeryczna)
<ol>
	<li>pozycja1</li>
	<li>pozycja2</li>
</ol>
Link w zdjęciu
<a href="Link wywołujący stronę" target="_blank >
  <img src="link do zdjęcia" alt="opis zdjęcia" />
</a>
Znacznik adress (pozycjonowanie strony)
<address>
Mail us: <a href="mailto:adres email">wyświetlany napis</a><br />
Call us: <a href="tel:+numer tel">wyświetlany napis</a><br />
</address>
Pobieranie z linku
<a href="ścieżka/do/pliku.cv" download="nazwa pliku"> opis</a>
ZNACZNIK OTWIERAJĄCY TREŚĆ (logo odsyłające do strony głównej)
<header></header>

Nawigacja strony (w nagłówku, poziom)
<nav></nav>

Przewiń do wybranego id
<a href="#id">nazwa nawigacyjnego przycisku</a>
<h1 id="id">nagłówek przypisany do id wyżej"</h1>

Główna zawartość strony -> UNIKALNA (BEZ NAGŁÓWKA, NAVI I st00pek ETC)
<main></main>

st00pka (zawiera info o prawach aut, linki do społeczności, kontakt itp)
<footer></footer> (logo mediów zawsze jako SVG!)

Znaczniki / mnemoniki
<strong></strong>
&lt; i &gt; do pogrubiania tekstu

Znacznik <em></em>
Uwypuklenie, podkreślenie

Lista bez kropek
<ul style="list-style-type: none;">

Stajlisz kolor inline
    <h1 style="color: orange;"></h1>
    <p style="color: cyan;"></p>

Stajlisz wbudowany
<style>
  h1 {color: tomato;}
  p {color: oragne;}
</style>

stajlisz z linku
(wymaga pliku styles.css w którym wprowadzimy stajlisz wbudowany (bez znacznika style))
<link rel="stylesheet" href="./css/styles.css" />

Stajlisz dla grup, zamiast id uzyj Class="nazwaklasy"
.nazwaklasy rgb(0, 0, 0)

Stajlisz dla list
ul a {color: rgb(13, 13, 17);}

stajlisz dziedziczony
.klasa > p{}

Style interaktywne
:focus {} (zmienia kolor wybierając element tabem)
:hover {}  (zmienia kolor po najechaniu)
:active {} (zmienia kolor przytrzymując klawisz na elemencie)

Waga selektórów (od najwyższej - decyduje podczas konfliktu, która reguła ma pierwszeństwo)
  inline
    id (#)
      classes, attributes, pseudo-classes (.)
        elements, pseudo-elements (p{color} ma mniejsza wartość niż np secion > p{color})

--!! jezeli wartość reguł jest taka sama, podczas konfliktu używana jest ostatnia reguła!!--
            Aby zwiększyć ważność reguły => !important (przykład poniżej)
                      p {color: orange !important;}

.post-link {color: inherit;} - Wartość inherit informuje przeglądarkę, że element musi dziedziczyć wartość właściwości z elementu nadrzędnego.