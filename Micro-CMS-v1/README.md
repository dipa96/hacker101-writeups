# Micro-CMS v1

## flag0

+ "New page", enumerare cambiando id

![picture](imgs/1.png)

+ "Edit page"

![picture](imgs/2.png)

Stesso ragionamento e flag trovata.

## flag1

+ testing per SQL injection

![picture](imgs/3.png)

## flag2

+ crea nuova pagina e inserisci payload xss nel titolo, poi ritorna su home

![picture](imgs/4.png)

## flag3

+ bottone presente in una pagina

![picture](imgs/5.png)

+ "Markdown is supported, but scripts are not" , posso creare un payload usufruendo del tag button e dell'event onclick

![picture](imgs/6.png)

+ <button onclick=alert(1)>pentestingmadesimple</button>

+ non appare nessuna flags, cercare nel codice sorgente della pagina

![picture](imgs/7.png)
