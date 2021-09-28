---
title: För juristen
layout: article
permalink: "/publicera/for-juristen"
---

## Vilka juridiska aspekter är viktiga att tänka på?

Innan man publicerar behöver man tänka på tre aspekter:

- **Sekretess​** – finns det uppgifter som borde vara sekretessbelagda i datan?
- **Upphovsrätt​** – finns det uppgifter som inte är våra?
- **Dataskydd​** – finns det personuppgifter i datan?

Svaret till dessa frågor bör vara **NEJ, NEJ och NEJ**.

## Hur publicerar man något ändå?

Om det finns data som borde vara sekretessbelagda eller personuppgifter måste man ta bort dessa från datamängden. Detta kan göra automatiskt med ett skript. Vissa offentliga aktörer har till exempel valt att ta bort enskilda företags organisationsnummer från sina leverantörsreskontra. Örebro kommun hade däremot valt i ett första skede att ha dem kvar eftersom samhällsnyttan bedömdes väga tyngre.

<i class="fas fa-info-circle"></i>
Genom att hjälpa vissa kommuner har vi tagit fram flera Python-skript som kan t.ex. ta bort personnummer eller döpa om vissa kolumner. Dessa finns på [Github](https://github.com/okfse/accounts-payable-converter) som öppen källkod och du får gärna återanvända dem. Du får även gärna [kontakta oss](mailto:openup@okfn.se) för att få hjälp för att anpassa dem efter ett annat format.
{:.info}
