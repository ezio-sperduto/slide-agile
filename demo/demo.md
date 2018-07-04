
<!-- .slide: data-background="#FFFFFF" -->
<!-- .slide: data-color="#333333" -->

## Demo Slide web
MarkDown + Reveal.js  
2018-07-02 Infosons - Ezio Sperduto

---

## Inizializzare le slide
1. creare repo o cartella su **GitHub**
2. caricare file testo vuoto **slide.md**
3. copiare file wrapper **index.html** che usa *Reveal.js* e punta a *slide.md*
4. mettere link-raw di *index.html* di GitHub su [https://rawgit.com/](https://rawgit.com/) per generare la presentazione
5. **lavorare su *slide.md* per ottenere la presentazione!!!**

---

## Formattazione
* *corsivo* `*corsivo*` (asterisco singolo)  
* **grassetto** `**grassetto**` (asterisco doppio)  
* ~~barrato~~ `~~barrato~~` (doppia tilde)   
*Esempio **che** combina* gli **stili** per ~~ottenere~~ un gran __risultato__.

---

## Intestazioni
Iniziare una riga con:  
**\#** equivale a marcare come `<H1>`  
**\##** equivale a marcare come `<H2>`  
**\####** equivale a marcare come `<H4>`  

---

## Link

Per i link automatici basta scrivere www.link.it  
Per link più elaborati è sufficiente:  
`[Testo mostrato](http://www.link.it)`  
E si ottiene [Testo mostrato](http://www.link.it)

---

## Citazioni

Si scrive così:
```
> C'era una volta
> in America...
```

per ottenere:
> C'era una volta  
> in America...

---

## Liste puntate
```
* Item 1
* Item 2
	* Item 2a
	* Item 2b
```
* Item 1
* Item 2
	* Item 2a
	* Item 2b

per la sottolista è necessario tabulare	

---

## Liste numerate
```
1. Item 1
2. Item 2
	* Item 2a
	* Item 2b
```
1. Item 1
2. Item 2
	1. Item 2a
	2. Item 2b

per la sottolista è necessario tabulare	

---

## Immagini
Logo di Git: ![Git Logo](git.jpg)  
La sintassi è uguale al link, ma preceduta dal punto esclamativo:
```
![Didascalia](/percorso/relativo/immagine.png)
```
---

## Regole extra

* per forzare l'accapo, mettere due spazi
* il carattere `\` permette di fare *escape* dei caratteri speciali

---

## Blocco di codice "verbatim"

Per i blocchi di codice monospaziato si usa il carattere **apice inverso** o **backtick**  
* per il blocco di codice *inline* è sufficiente un solo backtick `esempio` (\`esempio\`)
* per il blocco verticale occorre identificarlo con tre backtick  
\```  
blocco  
\```  

---

## Blocco di codice "verbatim"

* auto-highlight: specificare un linguaggio:  
\```java  
public interface Pippo{  
     abstract int somma(int a,int b);  
}  
\```  
  
per ottenere le parole chiave evidenziate:

```java
public interface Pippo{
	abstract int somma(int a,int b);
}
```
---
<!-- .slide: data-background="#FFFFFF" -->
<!-- .slide: data-color="#333333" -->
## Tabelle
Per le tabelle si possono usano **\| \- :**
```
Nome | Cognome | Telefono
------------ | :-------------: | ------------:
Steve | Jobs | 1234
Bill | Gates | 666
```
e il risultato è

Nome | Cognome | Telefono
------------ | :-------------: | ------------:
Steve | Jobs | 1234
Bill | Gates | 666

---

## HTML incorporato
E' possibile aggiungere HTML puro, e viene renderizzato correttamente:
```
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>
```
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

---
## Linee orizzontali

E' sufficiente usare 3 o più asterischi:  
\***  
per ottenere  
*******  

---

## Formule con *KaTeX*

KaTeX è una versione web di LaTeX. 

La *funzione* $\Gamma(n) = (n-1)!,\forall n\in\mathbb N$ è   
soddisfatta da:

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

---

## Formule con *KaTeX*
- la codifica delle formule è la stessa di LaTeX
- formule inline, dollaro singolo
- formula blocco, dollaro doppio
```
\$\Gamma(n) = (n-1)!,\forall n\in\mathbb N\$
```
---

<!-- .slide: data-background="#FFFFFF" -->
<!-- .slide: data-color="#333333" -->
<!-- svg: font-size="20px" -->

## Diagrammi con *mermaid*

<section class="diagram-slide">
    <span class="diagram-data" style="display:none;">
graph LR
A[Rettangolo] -- Arco --> B((Cerchio))
A --> C(Rett.smussato)
B --> D{Rombo}
C --> D
     </span>
     <!-- Diagram will be displayed in this DIV -->
    <div class="diagram-display"></div>
</section>

---
## Animazioni / Fragments

Premi avanti...

<p class="fragment">... per attivare ...</p>

<span class="fragment">... una slide con </span> <span class="fragment">**fragments**</span><span class="fragment">!!!</span>
---
## Animazioni / Fragments

Tipi differenti di **fragments**:

<p class="fragment grow">ingradimento</p>
<p class="fragment shrink">rimpicciolimento</p>
<p class="fragment fade-out">scomparsa</p>
<p class="fragment fade-up">comparsa (da sopra, sotto, destra o sinistra)</p>
<p class="fragment current-visible">comparsa e scomparsa</p>
<p>Evidenziazione <span class="fragment highlight-red">rosso</span> <span class="fragment highlight-blue">blu</span> <span class="fragment highlight-green">verde</span></p>

---
## Animazioni / Fragments
Per aggiungere un **fragment**,   
mettere un tag **p** o **span** con classe  
**fragment**:
```
<p class="fragment">...</p>
<span class="fragment">...</span>
```

---
## Animazioni / Fragments
Altre classi valide:
- fragment grow
- fragment shrink
- fragment fade-out
- fragment fade-up
- fragment current-visible
...
---

## Transizioni
Vari effetti di transizione...

---
<!-- data-transition="zoom" -->

## Transizioni: zoom
ciao
---

<!-- data-transition="slide" -->

## Transizioni: slide
---
<!-- data-transition="concave" -->

## Transizioni: concave
---
<!-- data-transition="fade" -->

## Transizioni: fade
---
