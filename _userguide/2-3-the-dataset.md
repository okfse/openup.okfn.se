---
title: Datastrukturen
layout: article
permalink: "/visualisera/utforska-datat-själv/the-dataset"
---

Än så länge har vi bara samlat datamängden leverantörsreskontra från flera offentliga aktörer. Under projektet har vi utforskat hur man kan publicera och återanvända andra typer av inköpsdata och så småningom kommer plattformen kunna värda dem också.

Datamängden leverantörsreskontra har vi strukturerat genom att använda MetaSolutions datastandard som används av ett flertal kommuner (kolumner 1 till 14). Vi har även fått mer data från vissa organisationer och då har vi valt att ha kvar den (kolumner 15 till 24). Därför innehåller vår tabell 25 kolumner, som beskrivs nedan.

1. **Avtal** - länk eller referens till det avtal som köpet grundar sig på. Nästan alltid tomt.
2. **Belopp** - fakturerat belopp, oftast i svenska kronor (SEK), annars är valutan i kolumnen **Valuta**.
3. **Datum** - datum när fakturan registrerades, oftast korrekt till dagen. När datamängden bara innehåller månaden har vi valt att datera alla fakturor till månadens första dag.
4. **Fakturanummer** eller faktura-id.
5. **Förvaltning** - enhet/avdelning/förvaltning som har gjort inköpet.
6. **Grund** - Notering om grunden för inköpet: direktupphandling, upphandling, ramavtal eller annat sätt.
7. **Kommun ID** - 30 / 5000
Résultats de traduction
kommunkod enligt [SCB](https://www.scb.se/contentassets/7a89e48960f741e08918e489ea36354a/kommunlankod-2021.pdf). Tomt om inte en kommun
8. **Konto Nr** - numret på det konto som ni har bokfört inköpet på.
9. **Konto Text** - namnet på det konto som ni har bokfört inköpet på.
10. **Köpare** - köparens organisationsnummer.
11. **Köpare Text** - köparens namnet.
12. **Leverantör** - leverantörens namn.
13. **Leverantör ID** - leverantörens organisationsnummer. Fältet är tömt om numret är ett personnummer (för enskildfirmor)
14. **Valuta** - Tomt om fakturan använder SEK.
15. **Ansvar Kod**
16. **Projekt Kod**
17. **Aktivitet Kod**
18. **Verksamhet Kod**
19. **Objekt Kod**
20. **Ansvar Kod**
21. **Projekt Kod**
22. **Aktivitet Kod**
23. **Verksamhet Kod**
24. **Objekt Kod**
25. **Unik** - I vissa datamängder har vi upptäckt duplikat som vi identifierar i den här kolumnen den här kolumnen (Obs! Om tom betyder det att vi håller på att bekräfta unikheten.)

I de flesta fall representeras en fakturera av en rad men vissa fakturor som betaldes av flera konton representeras av fler rader.
