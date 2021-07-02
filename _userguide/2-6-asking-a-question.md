---
title: Visualisera data
layout: article
permalink: "/visualisera/utforska-datat-själv/visualising-data"
---

I Metabase kan man skapa en visualisering genom att ställa en fråga till datan. Tryck på **Ställ en fråga** längst upp till höger på sidan.

Här kommer vi att titta på ett specifikt exempel på hur man ställer en fråga med den avancerade editorn.

**Example**
Låt oss säga att vi vill titta på hur mycket Eskilstuna Kommun har spenderat per månad under första halvåret 2020.

1. Tryck på **Ställ en fråga** och välj **Anpassad fråga**.

    ![](/assets/images/userguide/metabase-question-example-1.png)

2. Välj **Leverantörsreskontra**.

   ![](/assets/images/userguide/metabase-question-example-2-1.png)

   Välj **Leverantörsreskontra** igen.

   ![](/assets/images/userguide/metabase-question-example-2-2.png)

3. Filtrera data efter Köpare *Eskilstuna Kommun* och datum *January 1st 2020 till June 30th 2020*. Filtrera efter **Unik** för att se till att undvika att dubbelräkna fakturor. (Se [denna sida](/visualisera/utforska-datat-själv/filtering-the-data) för mer detalj om filtrering.)

   ![](/assets/images/userguide/metabase-question-example-3.png)

4. Under **Summera** väljer du vad du vill se, i detta fall *Summan av*.

   ![](/assets/images/userguide/metabase-question-example-4-1.png)

   Välj kolumnen som du vill tillämpa denna statistik på, i detta fall *Belopp*.

   ![](/assets/images/userguide/metabase-question-example-4-2.png)

5. Välj vad du vill gruppera efter, i detta fall **Datum**. Som förstahandsval kommer det en grupp per dag, men du kan välja t.ex. *Månad* istället. Sedan tryck på **Visualisera**.

   ![](/assets/images/userguide/metabase-question-example-5.png)

6. Nu kan du se din visualisering. Än så länge är det en linjediagram.. Tryck på **Visualisering** längst ned till vänster och välj **Stapel** för att få en stapeldiagram.

   ![](/assets/images/userguide/metabase-question-example-6.png)

7. Nu har vi en stapeldiagram! Det finns många saker man kan göra för att göra den snyggare och de finns i **Inställningar** längst ned till vänster. T.ex. kan du lägga till den totala summan ovanpå varje stapel. Tryck på **Visa** i **Inställningar** och välj **Visa värden på datapunkter**.

   ![](/assets/images/userguide/metabase-question-example-7.png)

8. Nu är vår visualisering klar!

   ![](/assets/images/userguide/metabase-question-example-8.png)

<i class="fas fa-info-circle"></i>
OBS! När du beräknar sammanfattningsstatistik, till exempel den totala summan som en viss köpare spenderar får du komma ihåg att filtrera efter **Unik** = *True*, annars kan du överskatta ditt värde eftersom vissa fakturor kommer räknas mer än en gång. Om du däremot vill se det totala beloppet registrerat på ett visst konto, ska du inte använda detta filter eftersom fakturor aldrig registreras mer än en gång per konto.
{:.info}

Om du vill skapa mer avancerade visualiseringar rekommenderar vi [Metabases dokumentation](https://www.metabase.com/docs/latest/users-guide/custom-questions.html) på engelska.
