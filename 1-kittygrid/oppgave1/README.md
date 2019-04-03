#Oppgave 1

html-filen vår er bygd opp av div'er med disse klassene:

```
<grid>
    <smallgrid>
        <desc>
            <textHolder/>
        <desc/>
        <photo/>
    <smallgrid/>
    
    <smallgrid>
            <desc>
                <textHolder/>
            <desc/>
            <photo/>
        <smallgrid/>
    .
    .
    .
<grid/>
```
I js-filen finnes en funksjon som setter klassen "even" og "odd" på annenhver div med smallgrid-klassen.
I css-filen er det en del stylingregler som er blitt kommentert ut for å fjerne støy slik at vi kan fokusere på egenskapene til css grid. 

I første omgang, ønsker vi å fordele 'photo' og 'desc' - diven vår i på en rad delt i tre kolonner.
1. Gi 'smallgrid' egenskapen til css-grid, ved å bruke display.
_Tips:_ Når du har satt `display: grid` på en klasse, så kan du bruke Inspect-verktøyet for å se hvordan gridfordelingen ser ut. 
2. Del opp 'smallgrid' i tre like kolonner, ved å bruke `grid-template-columns`. Dette blir gjort fordi vi ønsker at 'desc' skal strekke seg over 2 kolonner, mens 'photo' skal dekke 1 kolonne i neste oppgave.  

Neste steg er å endre på 'grid'. Slik at hver 'smallgrid'-div oppfører seg responsivt avhengig av hvor mye plass det er på skjermen. 
3.  Fordel grid i kolonner igjen med , der en kolonne er minimum 350px og max ``1fr`` vha ``repeat()`` og ``auto-fill``.
4. Gi radene i grid 15px mellomrom vha ``grid-row-gap``.

Prøv å endre på størrelsen til skjermen din, og se hvordan kolonnene endrer seg. 