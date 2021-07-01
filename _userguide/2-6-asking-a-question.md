---
title: Visualising data
layout: article
permalink: "/visualisera/utforska-datat-själv/visualising-data"
---

In Metabase, you make a visualisation by asking a question to the data. You can access this function at any point by clicking the **Ställ en fråga** at the top right corner of the page. 

Here we will look at a specific example of asking a question using den avancerade editorn.

**Example**
Let's say we want to look at how much Eskilstuna Kommun has spent per month during the first half of 2020. 

1. Click on **Ställ en fråga** and select **Anpassad fråga**. 

    ![](/assets/images/userguide/metabase-question-example-1.png)

2. Select **Leverantörsreskontra**.

   ![](/assets/images/userguide/metabase-question-example-2-1.png)

   In the following screen select **Leverantörsreskontra** again.

   ![](/assets/images/userguide/metabase-question-example-2-2.png)

3. We then filter the data set so that we get data from *Eskilstuna Kommun* between *January 1st 2020 and June 30th 2020*. Here we also add a filter requiring that **Unik** is true so that we make sure we are counting each invouce only once. (For more details on filtering please refer to [this section](/visualisera/utforska-datat-själv/filtering-the-data).)

   ![](/assets/images/userguide/metabase-question-example-3.png)

4. Then under **Summera** we select the metric that we want to look at, in this case *Summan av*. 

   ![](/assets/images/userguide/metabase-question-example-4-1.png)

And then we select the column that we want to apply this metric to, in this case *Belopp*. 

   ![](/assets/images/userguide/metabase-question-example-4-2.png)

5. We select which column we want to group by, in our example, **Datum**. By default the data is shown per day, so we click on *per dag* and then select *Månad* instead. Then click on **Visualisera**. 

   ![](/assets/images/userguide/metabase-question-example-5.png)

6. Now you can see your graph. By default this is displayed as a line graph but in our example it would be better to have a bar chart. Click on **Visualisering** at the bottom left of the page and then select **Stapel**. 

   ![](/assets/images/userguide/metabase-question-example-6.png)

7. Now that we have our bar chart we can change the settings by clicking on **Inställningar** at the bottom left of the page. As an example here we will add the total sum for each month at the top of each bar. For that we click on the **Visa** tab within **Inställningar** and then toggle the button under **Visa värden på datapunkter**. 

   ![](/assets/images/userguide/metabase-question-example-7.png)

8. And now we have our chart! 

   ![](/assets/images/userguide/metabase-question-example-8.png)

<i class="fas fa-info-circle"></i>
OBS! When calculating summary statistics such as the total sum spent by a given buyer, please remember to apply a the **Unik** is *True* filter, otherwise you might overestimate your value since you could be counting a given invoice more than once. If, on the other hand, you would like to see the total amount registered to a specific account, you should not apply this filter since invoices are only ever registered to a given account once.  
{:.info}

For a complete guide on how to ask more complex questions to the data set, please refer to [this Metabase tutorial](https://www.metabase.com/docs/latest/users-guide/custom-questions.html). 