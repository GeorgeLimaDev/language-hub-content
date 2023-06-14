---
title: Relevance
id: 1qlObWIib6KqgrfX1FCOXS
status: PUBLISHED
createdAt: 2020-04-14T13:35:28.989Z
updatedAt: 2023-01-23T13:48:19.938Z
publishedAt: 2023-01-23T13:48:19.938Z
firstPublishedAt: 2020-04-14T23:58:35.468Z
contentType: trackArticle
productTeam: Marketing & Merchandising
slug: relevance
trackId: 19wrbB7nEQcmwzDPl1l4Cb
trackSlugEN: vtex-intelligent-search
---

**Relevance settings** define the order in which products are shown in search results. The order changes according to the criteria and priorities configured for the Search Engine.

Relevance rules are applied to the search results only when the results are sorted by relevance in your store's search. For example, if a customer sorts results by price, relevance settings will not be considered when displaying search results.

You can configure relevance in two ways:

  - __Priority criteria__: it imposes that one or more criteria has a higher priority among the others. In this situation, there are no weights; all products that have this feature will be shown first in the search results.
  - __Criteria composition__: it is a way to distribute weights for each option, ranging from 0 to 10. Here, there is no order between the criteria; the weights will define the relevance.

![regras-relevancia-1-EN](//images.ctfassets.net/alneenqid6w5/pWaOZBllEtnkrAxc2kEdJ/7ed55448e3b78b749a8d6d0c7d0d803b/Captura_de_Tela_2022-03-25_a__s_15.17.28.png)

The information considered for the relevance is:

- __Discount (from/to)__: it compares the [List Price](https://help.vtex.com/en/tracks/precos-101--6f8pwCns3PJHqMvQSugNfP/3XcXp0r5WrJvogB8KIX4Kx#list-price) and the [Base Price](https://help.vtex.com/en/tracks/precos-101--6f8pwCns3PJHqMvQSugNfP/3XcXp0r5WrJvogB8KIX4Kx#definition) to determine whether the product will be classified as having a discount.
- __Release date__: this criterion assigns an automatic decreasing value (between 1 and 0) to the product, based on the date it was added to the catalog and considering a 90-day interval. Products added to the catalog today would have the value 1. This value would decrease every day until it becomes 0 after 90 days. This value will be multiplied by the weight you assign to the __Release date__ criterion to compose product relevance.
- __Best sellers__: number of orders for the product in the last 90 days.
- __Best sellers by revenue__: the total revenue generated by the product in the last 90 days.
- __Popularity__: the number of clicks the item received in the last 90 days.
- __Promotion__: it checks for [Campaign Audiences](https://help.vtex.com/en/tutorial/overview-2--tutorials_326?&utm_source=autocomplete#campaign-audiences) or [Promotions](https://help.vtex.com/en/tracks/promocoes--6asfF1vFYiZgTQtOzwJchR/2a2D0K85Ahvs4hLnL3Ag7N#) linked to the item to determine whether the product will be classified as a promotion.
- __Catalog Score__: Catalog sorting tie-breaker based on the value given to products. Learn more about the Score field [in this article](https://help.vtex.com/en/tutorial/how-does-the-score-field-work--1BUZC0mBYEEIUgeQYAKcae).
- __Available matrix variety__: Relevance is based on the percentage of SKUs available per product. In a scenario where _Product A_ has 3 SKUs and 3 of them are available, and _Product B_ has 5 SKUs and 2 of them are available, _Product A_ stands out over _Product B_ because the percentage of SKUs is higher.

The set of weights and criteria distribution generates a score for the product, which determines its position in the search result ranking.

<div class="alert alert-warning">
  <p>IIf you want to use priority criteria, we recommend adding only one criterion in this field. Adding more criteria compromises the ordering or search results, since only the first criterion will be considered.</p>
</div>

So you can tailor the behavior of the search results to a specific strategy. For example: A fashion store receives new collections frequently. The retailer chooses to prioritize new products instead of products with discounts. To do that, the tool can be configured as follows:

<b>Priority criteria:</b>
<ul><li>Empty</li></ul>
<b>Criteria composition:</b>
<ul><li> <b>Popularity:</b> 7</li>
    <li> <b>Release date:</b> 10 </li>
    <li> <b>Best sellers:</b> 6</li>
    <li> <b>Best sellers by revenue:</b> 6</li>
    <li> <b>Promotion:</b> 0 </li>
    <li> <b>Discount:</b> 0 </li>
    <li> <b>Variation availability (SKU):</b> 10 </li></ul>

If this retailer wants new products to always have the highest priority, there are two ways to configure the Relevance rules:

<ol>
    <li> <b>Priority criteria:</b> </li>
   <ul><li> <b>Release date</b></li></ul>
     <b>Criteria composition:</b>
   <ul><li> <b>Popularity:</b> 7</li> 
   <li> <b>Best sellers:</b> 6</li> 
   <li> <b>Best sellers by revenue:</b> 6 </li> 
   <li> <b>Promotion:</b> 0 </li>
   <li> <b>Discount:</b> 0 </li>
   <li> <b>Variation availability (SKU):</b> 10 </li></ul><br>
    <li> <b>Priority criteria:</b> </li>
    <ul><li>Empty</li></ul>
    <b>Criteria composition</b>
    <ul> <li> <b>Popularity:</b> 0 </li>
    <li> <b>Release date:</b> 10 </li>
    <li> <b>Best sellers:</b> 0 </li>
    <li> <b>Best sellers by revenue:</b> 0 </li>
    <li> <b>Promotion:</b> 0 </li>
    <li> <b>Discount:</b> 0 </li>
    <li> <b>Variation availability (SKU):</b> 0 </li></ul>
</ol>

## Configuring relevance rules

To change relevance settings, follow the steps below.

1. In the Admin, go to the **Storefront** module.
2. In **Intelligent Search**, click **Relevance Rules**.
3. Choose the criterion whose weight you want to change.
4. Click the <i class="fas fa-minus"></i> or <i class="fas fa-plus"></i> icons to set a number. If you want to change a criterion from **Criteria composition** to **Priority criteria**, click on the <i class="fas fa-grip-vertical"></i> icon and drag it to the top of the page, as shown below. Note that when the criterion is set as a priority, you can no longer change its weight. 
![regras-relevancia-EN](//images.ctfassets.net/alneenqid6w5/iZze1vchSYf9lLFJnfwiT/892c2f6f5aca868508c1a7f0c48a27d8/regras-relevancia-EN.gif)
5. Click `Save` to finish.
