---
title: Filtering the data
layout: article
permalink: "/visualisera/utforska-datat-själv/filtering-the-data"
--- 

One of the most useful features of Metabase is that it allows you to filter the dataset and look more closely at the data you are interested in. 

You can filter by clicking on the ***Filter*** purple button at the top left of the page and choosing which columns to filter on. You can filter by köpare, leverantör, datum, belopp, konto and more. 

![](/assets/images/userguide/metabase-filtering.png)

When searching for a particular leverantör it is recommended that you use **Levenrantör ID** rather than **Leveräntor** since the leverantör might be referred to by slightly different names in different fakturor. Similarly, filtering by **Konto Nr** usually gives cleaner results than filtering by **Konto Text**.

<i class="fas fa-info-circle"></i>
If you would like to see which state buyers have data on the platform you can click **Filter**, select **Köpare Text** and a list of all buyers will be displayed.
{:.info} 

![](/assets/images/userguide/metabase-kopare-list.png)


## Example

Let's say we want to look at which services Mora Kommun has bought from Telenor during March 2020. 

1. Filter by **Köpare Text** and select *Mora Kommun*. 

    ![](/assets/images/userguide/metabase-filter-example-1.png)

2. Filter by **Datum**. On the left dropdown menu select *Mellan* and then choose the dates between the first and the last days in March 2020. 

    ![](/assets/images/userguide/metabase-filter-example-2.png)

3. Now we want to add a final filter so that we get the invoices from Telenor. As mentioned before, the best way to filter on leverantör is by using **Leverantör ID**. Since we don't necessarily know the organisationsnummer of Telenor, we can find a row in the table where **Leverantör** is Telenor, click on the corresponding **Leverantör ID** and then click the equals sign in the pop up box with the filter icon. 

    ![](/assets/images/userguide/metabase-filter-example-3.png)

4. Now the table has all the right filters and is displaying our chosen subset of data.

    ![](/assets/images/userguide/metabase-filter-example-4.png)