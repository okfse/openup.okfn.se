---
title: The Dataset
layout: article
permalink: "/visualisera/utforska-datat-själv/the-dataset"
---

The dataset contains 25 columns, as described below. In the data, each row corresponds to an invoice, but not all rows in the dataset represent a unique invoice. For instance, two rows might correspond to the same invoice being assigned to two different accounts.

1. **Avtal** - länk eller referens till det avtal som köpet grundar sig på. This information is almost always left empty. 
2. **Belopp** - the amount invoiced, generally in SEK unless otherwise stated under **Valuta**.
3. **Datum** - datum när fakturan registrerades, generally accurate to the day. For Göteborg, Eskilstuna, Örebro and Umeå the dates published only specificy the month, so we have assumed that all expenses occurred on the first day of the month. Most datasets contain data ranging from January 2019 to June 2020. There is more recent data for Eskilstuna, Umeå and DIGG - Myndigheten för digital förvaltning. More recent data will be added soon for Örebro and Göteborg.
4. **Fakturanummer** eller faktura-id.
5. **Förvaltning** - enhet/avdelning/förvaltning som har gjort inköpet. This information is rarely available. 
6. **Grund** - Notering om grunden för inköpet: direktupphandling, upphandling, ramavtal eller annat sätt. Generally left empty in this dataset.
7. **Kommun ID** - municipality code according to [this numbering](https://www.scb.se/contentassets/7a89e48960f741e08918e489ea36354a/kommunlankod-2021.pdf). This field is left empty when the buyer is not a municipality. 
8. **Konto Nr** - numret på det konto som ni har bokfört inköpet på. This information is not always available. 
9. **Konto Text** - namnet på det konto som ni har bokfört inköpet på. This information is not always available.
10. **Köpare** - köparens organisationsnummer.
11. **Köpare Text** - köparens namnet.
12. **Leverantör** - leverantörens namn. 
13. **Leverantör ID** - leverantörens organisationsnummer. If the leverantör is a private person with an enskild firma, the personnummer is remove before the data is uploaded for privacy reasons. This information is not always provided. 
14. **Valuta** - sometimes left empty if the currency is SEK. 
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
25. **Unik** -  this column was added to address the fact that not every row corresponds to a different invoice. If Unik is True that row is a unique transaction, if it is False the row corresponds to a transaction that has already appeared in the dataset. (Note: In some cases Unik is left empty because that particular data has not yet been updated to include this column.)

Columns 15 to 24 refer to specific reporting fields used by kommuner, myndigheter and regioner to specify a greater level of detail for each invoice. These fields are usually not reported but they can contain very interesting information when provided.

Now let's dive into the data! 
 
