---
title: Filtrera data
layout: article
permalink: "/visualisera/utforska-datat-själv/filtering-the-data"
---

Med Metabase kan du filtrera data och titta närmare på precis det du är intresserad av.

När du bläddrar i data kan du filtrera genom att trycka på knappen ***Filter*** längst upp till höger välja vilka kolumner du vill filtrera efter. Du kan t.ex. filtrera efter köpare, leverantör, datum, belopp, konto...

![](/assets/images/userguide/metabase-filtering.png)

När du letar efter en viss leverantör rekommenderas att du använder **Levenrantör ID** istället för **Leveräntor** eftersom deras exakta namn kan variera. På samma sätt ger filtrering efter **Konto Nr** vanligtvis renare resultat än filtrering efter **Konto Text**.

<i class="fas fa-info-circle"></i>
Om du vill se listan på alla offentliga inköpare på plattformen kan du trycka på **Filter** och välja **Köpare Text**.
{:.info}

![](/assets/images/userguide/metabase-kopare-list.png)
## Example

Låt oss säga att vi vill se vilka tjänster Mora Kommun har köpt från Telenor under mars 2020.

1. Filter efter **Köpare Text** och välj *Mora Kommun*.

    ![](/assets/images/userguide/metabase-filter-example-1.png)

2. Filter efter **Datum**. Välj *Mellan* och för start- och slutdatum 1a och 31a mars

    ![](/assets/images/userguide/metabase-filter-example-2.png)

3. Nu vill vi filtrera efter leverantör. För att hitta Telenors organisationsnummer kan man gå till deras webbplats, googla det eller leta efter en faktura från telenor genom att filtrera efter **Leverantör**. Sen kan man trycka på Telenors **Leverantör ID** och välja likhetstecken för att filtrera efter Telenors organisationsnummer.

    ![](/assets/images/userguide/metabase-filter-example-3.png)

4. Nu har man valt alla relevanta filter och man kan se Telenors fakturor till Mora kommun i mars 2020.

    ![](/assets/images/userguide/metabase-filter-example-4.png)
