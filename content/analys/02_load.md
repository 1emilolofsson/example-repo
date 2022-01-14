---
Title: LOAD
Description: Test 
Template: analys
---

# UTVÄRDERING AV TRE WEBBPLATSERS LADDNINGSTID OCH ANVÄNDBARHET

I den här rapporten kommer jag att gå igenom tre valda webbplatsers laddningstid och användbarhet. Jag kommer att testköra webbplatserna för att 

URVAL
-----------------------
Webbplatserna jag valt för denna undersökningen är Aftonbladet, Expressen och Dagens nyheter. Dessa val har gjorts dels för att alla sidorna är tidningar och kan därför jämföras på ett mer "rättvist" sätt. De har liknande funktioner, det vill säga bilder, text och eventuella klipp vilket kanske kan underlätta för undersökningen. På varje sida har jag valt att göra mätningarna på förstasidan.

<div>
    <a href="%base_url%/image/aftonbladet.png" target="_blank"><img
    src="%base_url%/image/aftonbladet.png?h=250&w=500" alt="aftonbladet"></a>
    <a href="%base_url%/image/dn.png" target="_blank"><img
    src="%base_url%/image/dn.png?h=250&w=500" alt="dn"></a>
    <a href="%base_url%/image/expressen.png" target="_blank"><img
    src="%base_url%/image/expressen.png?h=250&w=500" alt="expressen"></a>
</div>

METOD
-----------------------
För att utvärdera webbplatserna kommer jag använda mig av verktyget Pagespeed insights som jag kör sidorna genom för att se vilka betyg de får där. Mätningarna kommer göras både för Desktop och Mobile. Jag kommer sedan placera mätningarna och värdena i ett excel-ark och jämföra. För varje sida kommer mätningar göras för att inspektera hur sidan laddar och vilka resureser som används.

MÄTNINGAR
-----------------------

<iframe width="700px" height="300px" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vT5wCjHoCN6qyBZGyCga21tJbclWgju2W7oGJ5OEF2DJyufDnJ6cLIPshB0STAB3g/pubhtml?gid=936536194&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

RESULTAT
-----------------------

Detta är då en sammanställning av mätningarna jag gjort på sidorna. Betygen visar att sidorna generellt har relativt liknande laddnings-värden. Prestandan får högre siffror i desktopen på alla sidor, vilket kanske inte var helt oväntat. Aftonbladets prestanda-betyg leverar sämre än de andra tidningarna, där deras 56 ställer sig mot nästan 100 i betyg hos de andra. First content paint leverar alla sidor en snabb laddningstid men i exempelvis time to interactive är siffrorna högre precis som total blocking time som ligger över 2000 ms i mobile på Expressen och Aftonbladet. 

__Mätningarna i devtools flik networks__

__aftonbladet:__
64 förfrågningar
1.0 MB har överförts
4.3 MB resurser
Läs in: 2.73 sek

__Dn:__
251 förfrågningar
2.1 MB har överförts
6.4 MB resurser
Läs in: 1.54 sek

__Expressen:__
58 förfrågningar
616 kB har överförts
2.7 MB resurser
Läs in: 2.37 sek

ANALYS OCH VINNARE
-----------------------

Alla sidor har liknande förbättringspunkter. Deras sidor har liknande upplägg med mycket bilder. De möjligheter som finns för aftonbladet att spara laddningstid ligger framförallt i att reducera Javascripts som inte används. Sedan är mycket av laddningtiden ett resultat av laddning av bilder där bilder skulle kunna skickas i modernare bildformat och kodas effektivare. Det var liknande på både desktop och mobile, men mobile hade mycket kraftigare laddningar. Expressen hade liknande men utöver det finns möjlighet att minska första serverns svarstid. Se till att serverns svarstid för huvuddokumentet är kort, eftersom alla andra förfrågningar är beroende av det. Liknande med Dagens nyheter, möjligheter till förbättring av servers svartid och javascript reducering. Hos alla är det aktuellt att minska påverkan från tredjepartskod. 

Dagens nyheter levererade bäst i nästan alla kategorier. Även fast de hade mest resurser att ladda in.

REFERENSER
-----------------------

https://www.aftonbladet.se

https://www.expressen.se

https://www.dn.se


Övrigt
-----------------------

En text av Emil Olofsson.