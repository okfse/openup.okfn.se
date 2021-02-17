---
title: Visma Proceedo
layout: article
permalink: "/publicera/exportera-data-manuellt/visma-proceedo"
---

I Visma Proceedo finns det ett rapportverktyg som vi kommer använda för att skapa en mall. Den här mallen kommer sedan användas för att exportera flera dataserier.

1. Öppna rapportverktyget genom att trycka på **Rapporter** i toppmenyn.

    ![](/assets/images/guide/proceedo/visma-proceedo-0.png)

2. Du kommer in till en sida som heter **Rapportgenerator**. Där kan du även trycka på knappen **Ny rapportfråga (1)**.

    ![](/assets/images/guide/proceedo/visma-proceedo-1.png)

3. I **Datakälla** får du välja tabellen som innehåller listan på dina fakturor **(2)**. Efter det kan du välja vilka kolumner **(3)** du vill lägga till i din rapport genom att trycka på pilen **(4)**.

    Här ska man vara så nära som möjligt [standarden](https://lankadedata.se/spec/leverantorsreskontra/) som togs fram inom projektet NSÖD. Varje organisation använder sina egna namn för kolumnerna så ni måste bedöma vilka är de rätta i din kontext. Det är också sannolikt att du inte hittar alla kolumner i Proceedo och vi förklarar hur man kan lösa det efter filen är skapad.

    Här finns kolumnerna sammanfattade:
    * ***kopare***:​ er organisations organisationsnummer
    * ***faktura_nr***​: fakturanummer
    * ***leverantör​***: leverantörens namn som text
    * ***leverantör_id​***: leverantörens organisationsnummer
    * ***forvaltning​***: här kan du också välja Projekt om det passar bäst er interna struktur
    * ***konto_nr​***: Kontonumret
    * ***konto_text***​: Kontobeskrivning eller liknande
    * ***belopp***
    * ***valuta​***: behövs bara om ni har fakturor med andra valutor än SEK
    * ***datum***:​ vi rekommenderar att använda datumet när fakturan registreras
    * ***grund​***: specificerar om fakturan kommer från en direktupphandling, ramavtal...
    * ***avtal​***: en länk till dokument som ger mer detalj om inköpet
    * ***kommun_id***​: om organisationen är en kommun, SCBs kommun ID
    * ***ansvarskod***
    * ***projektkod***
    * ***aktivitetskod***

4. Lägg till så många kolumner som du kan. Om du inte hittar t.ex. kolumnen **köpare** eller **kommun_id** kommer vi lägga till dem i efterhand eftersom alla rader kommer innehålla samma värde.

5. Om du vill filtrera bort fakturorna som är sekretessbelagda eller fakturorna som inte blev godkända kan du välja fler kolumner om detta status och använda dem för att filtrera exporteringen. På skärmbilden nedan har vi filtrerat alla fakturor med huvudstatus OK och med sekretess N (för nej). Dessutom har vi otickat checkboxen så de här kolumnerna inte exporteras.

    ![](/assets/images/guide/proceedo/visma-proceedo-2.png)

6. När du har alla kolumner du behöver kan du ge ett namn till din rapportfråga och spara den.


7. Nu kan du välja en tidsram för att exportera en första fil. Börja med ett avslutat år som 2019. För att begränsa exporteringen till detta år får du filtrera efter din datumkolumn, med startdatum *2019-01-01* och slutdatum *2019-12-31*.

    ![](/assets/images/guide/proceedo/visma-proceedo-3.png)

8. Nu kan du trycka på **Skapa rapport**.

    ![](/assets/images/guide/proceedo/visma-proceedo-4.png)

9. Och ladda ner filen från sidan **Skapade rapporter**.

    ![](/assets/images/guide/proceedo/visma-proceedo-5.png)

10. Byt start- och slutdatum för att skapa en fil per önskad tidsram.

11. När alla dina filer är exporterade kan du öppna dem i Excel och lägga till de kolumnerna som saknades i Proceedo. När informationen saknas kan du lämna dem tomma. För kopare och kommun_id kan du skriva ert organisationsnummer och er [kommunkod](https://www.scb.se/hitta-statistik/regional-statistik-och-kartor/regionala-indelningar/lan-och-kommuner/lan-och-kommuner-i-kodnummerordning/) i alla rader. Glöm inte att döpa om alla kolumner till namnen som står i Metasolutions [standard](https://lankadedata.se/spec/leverantorsreskontra/).

12. Efter det kan du granska din data för att se till att det inte finns något misstag eller personuppgifter. Du kan t.ex. söka för personnummer i Excel

13. Sista steget är att exportera din data till CSV och att publicera det! Grattis!
