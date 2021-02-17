---
title: För IT-strategen
layout: article
permalink: "/publicera/for-it-strategen"
---

## I vilken format ska man publicera datan?

**Open Contracting Data Standard** (OCDS) är den internationella standarden för att publicera öppna upphandlingsdata. Den skapades av Open Contracting Partnership precis för detta syfte och används av tiotals länder och andra organisationer, bl.a. Norge och Finland. Man kan läsa mer om standarden [här](https://www.open-contracting.org/data-standard). Inom projektet Open Up! studerar vi möjligheterna att använda OCDS men det är hittills ingen organisation i Sverige som har börjat att använda den.

Det här är en lista (på engelska) av alla typer av dokument och uppgifter som kan publiceras med OCDS:

![](/assets/images/OCP-standard-cycle.png)

Open Contracting har utarbetat en [mall](https://docs.google.com/document/d/1VAKw8QCU08__qUnssmbSl_N38Rpd7nhcNChZ80qHOCI/edit#) för att identifiera de tillgängliga källorna och kvaliteten på datan som kan öppnas upp, samt för att kartlägga tekniska alternativ för datapublikation (Open Contracting Data Standard Technical Assessment Template).

### Datastandard för leverantörsreskontra

För **leverantörsreskontra** finns det svenska standarder som togs fram av de aktörerna  som redan publicerar den här datamängden. Vi rekommenderar [MetaSolutions standard](https://lankadedata.se/spec/leverantorsreskontra/), som används inom NSÖD och liknar formaten valt av Umeå och Göteborg.

## Hur bygger jag ett hållbart dataflöde för att publicera datan?

Att exportera data manuellt regelbundet är krångligt och man vill gärna automatisera processen så mycket som möjligt. För detta måste man använda IT-system som heter ETL för att automatisera exporteringen av data från ett upphandlingsystem och/eller ekonomisystem.

Flera lösningar finns på marknaden men de mest populära inom offentliga organisationer är TietoEvry TEIS, Mulesoft Anypoint och Microsoft Biztalk. Inom projektet NSÖD håller man på att testa en automatisering med den första. Vi kommer uppdatera den här guiden.

<i class="fas fa-info-circle"></i>
Vi kommer uppdatera den här guiden så snart vi får tag på NSÖDs första prototyp. Om du jobbar för en organisation som vill eller har redan lyckats automatisera sitt dataflöde får du gärna kontakta oss så vi kan hjälpa och skriva om det i denna dokumentation.
{:.info}
