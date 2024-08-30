---
title: 'Received SKUs'
id: 4hxDUmbgOEVFSTU2Eqi8DK
status: PUBLISHED
createdAt: 2024-04-29T13:48:12.818Z
updatedAt: 2024-06-25T19:27:37.735Z
publishedAt: 2024-06-25T19:27:37.735Z
firstPublishedAt: 2024-04-29T14:16:25.091Z
contentType: tutorial
productTeam: Channels
author: 2p7evLfTcDrhc5qtrzbLWD
slug: received-skus-beta
locale: en
legacySlug: received-offers
subcategory: 
---

The Received SKUs page provides a way for [marketplaces](https://help.vtex.com/en/tutorial/visao-geral-marketplace--40Zd0z9h2RXsM9uMUp3kEb) to view, prioritize, and catalog items sent by the sellers. This way, they can create new products and link them to existing SKUs or products to make them available for sale. You can access this page on the VTEX Admin by going to Marketplace > Received SKUs or typing Received SKUs in the Admin search bar.  

Cataloging can be done manually or automatically [using one or more matchers](https://help.vtex.com/en/tutorial/entendendo-a-pontuacao-do-vtex-matcher?locale=pt) or [autoApprove](https://developers.vtex.com/docs/api-reference/marketplace-apis-suggestions/#put-/suggestions/configuration/autoapproval/toggle). You can also use third-party tools to do this.  

This article provides an overview in the sections [Page structure](#page-structure), [Cataloging priority](#cataloging-priority), and [Cataloging items](#cataloging-items).  

## Page structure  

The Received SKUs page is divided in tabs that correspond to the different offer statuses:  

- [Pending](#pending)  
- [Issues](#issues)  
- [Approved](#approved)  
- [Processing](#processing)  
- [Blocked](#blocked)  

Each tab displays a SKU list, offer SKU specifications, and the percentage of offers that have that status. Additionally, the tab has filter options that you can apply to the offers.  

![received-skus-tabs-en](https://images.ctfassets.net/alneenqid6w5/4jNrRvJsZgja1LuSz204P1/09fa16e993ba58dffa27b8809bb22c8f/received-skus-tabs-en.png)

### Pending

In the __Pending__ tab, you can see a list of all offers sent by a seller that haven't been approved yet. Offers can be filtered by __Seller, Category, Brand, and Inventory.__ Offer actions in this tab include: __Create new product, Link to product or SKU, Reject for correction, or Reject and block.__  

Each row in the list represents a product and contains the following information:  

- __Offer:__ Name of the product.  
- __SKU ID:__ Identification number of the product.  
- __Seller:__ Name of the seller who sent the offer.  
- __Category:__ Category the product is linked to, if it's already mapped. Otherwise, it will show as Unmapped.  
- __Price:__ Price of the product sent by the seller.  
- __Inventory:__ Number of products available in stock.  

To check all the specifications of a product, click the name of the product. This will open a window that contains all the product information.  

![received-skus-tabs-en](https://images.ctfassets.net/alneenqid6w5/3QSXyYXqhdAB3R4J3lL749/ff94df985c2cc930548645ac0fbd5e98/received-skus-analyse-product-en.png)

### Issues  

The __Issues__ tab contains all the offers that haven't been approved because they have issues that need to be corrected by the seller. The filters, actions, and identification fields of the Issues tab are similar to the ones in the __[Pending](#pending)__ tab.  

>ℹ️ The **Issues** tab doesn't have the option to request a correction.

To identify the issue of an offer, simply click the name of the product. This will open a window with the product information, an error message, and the offer reviewer.  

![received-skus-problems-tab](https://images.ctfassets.net/alneenqid6w5/4yZtOcq16r6SXvai0lWzau/58d57ab4904c6794299855c91bfa6ef1/received-skus-problems-tab.png)

### Approved  

The __Approved__ tab shows the received and approved offers. You can __Edit the product, View the product page,__ and __Filter products by Seller, Category, and Brand.__

Each row in the list represents a product and contains the following information:  

- __Offer:__ Name of the product.  
- __SKU ID:__ Identification number of the product.  
- __Seller:__ Name of the seller who sent the offer.  
- __Category:__ The category the product belongs to.  

### Processing  

The __Processing__ tab contains Received SKUs that are being evaluated by the VTEX system.  This is only a view tab. You can filter by __Seller__ and __Submitted Date.__

Each row in the list represents a product and contains the following information:  

- __Offer:__ Name of the product.  
- __SKU ID:__ Identification number of the product.  
- __Seller:__ Name of the seller who sent the offer.  
- __Submitted Date:__ Date when the offer was sent to the marketplace.  

>ℹ️ The offers in this tab are being evaluated by Matcher and Offer Quality or autoApprove, if they're configured. After evaluation, the offer can be sent to the **Pending, Issues, Approved, or Blocked** tabs, depending on the requirements.

### Blocked  

In the __Blocked__ tab, you can see the offers that were sent by the seller that have been blocked by the marketplace. You can __Unblock__ an offer, as well as filter by __Seller__ or __Reviewer.__  

Each row in the list represents a product and contains the following information:  

- __Offer:__ Name of the product.  
- __SKU ID:__ Identification number of the product.  
- __Seller:__ Name of the seller who sent the offer.  
- __Reviewer:__ Name of the agent that reviewed the offer.  

## Cataloging priority  

The Received SKUs list was developed to prioritize and streamline cataloging items. When you click any SKU in the list, you will see an overview of the SKU details in a sidebar, without leaving the list page. The sidebar also includes the match percentage assigned to the SKU by the matcher installed in your store.  

Some features that help prioritization are:  

### Filters  

Each tab described in the section above allows combining filters to create a SKU view.  

For example, if you select brand "ABC" and the "Socks" category, the view will display all SKUs of brand "ABC" that belong to the "Socks" category.  

Keep in mind that filter options are based on the SKUs available in the list. Suppose, for example, that the marketplace is connected to Seller A, B, and C, but there are only pending SKUs from Seller B and C. This means that the applied filters in the [Pending](#pending) tab will only show results from Seller B and C.  

### Sorting  

By default, the items that were submitted most recently are displayed at the top. However, you can also sort them by __Price__ and __Inventory__.  

In this case, the items will be sorted in ascending or descending order when you click the __Price__ or __Inventory__ column headers.  

![received-skus-ord-en](https://images.ctfassets.net/alneenqid6w5/3Eur3cPCdSTtZjoGIqeq6o/585afe9679294087fe9351cea7f0799a/received-skus-ord-en.png)

## Cataloging items  

All the SKUs displayed in the list are available for cataloging. However, we recommend [mapping the categories and brands](https://help.vtex.com/pt/tutorial/mapeamento-de-categorias-e-marcas-para-marketplace-vtex-beta--6NU8LwR6i0tTb8nk30bnbE) before this step to streamline the cataloging process.  

>⚠️ The offers in the Pending tab are only available for 30 days. After this period, they automatically expire and the seller will need to submit them again.

### Cataloging options

To catalog an offer, access the __Received SKUs__ page on the VTEX Admin by going to __Marketplace > Received SKUs__ or typing __Received SKUs__ in the Admin search bar.  

>ℹ️ All the offers on the Pending tab can be cataloged individually or in bulk.

The available cataloging actions are:  

- __Create new product:__ Creates a new SKU in the catalog and, consequently, a new product. We recommend using this option when a product doesn't exist in the marketplace catalog. To apply this action, follow the steps below:  

1. 	Select the desired SKUs.  
2. 	Click the <i class="fas fa-plus" aria-hidden="true"></i> Create new product button.  
3. 	Complete the Category and Brand fields for each product. If the mapping was previously completed, the fields will be filled automatically.  
4. 	Click `Approve`.  

>ℹ️ This action can be applied in the offer tabs **Pending** and **Issues**.

![received-skus-create-new-product-en](https://images.ctfassets.net/alneenqid6w5/4H2vmekbrtbXQXUVrwVoSF/2d18fb18e7711cb4cd341795ac0820b4/received-skus-create-new-product-en.png)

- __Link to an existing product:__ Creates a relationship between the seller product and a product in the marketplace catalog. To apply this action, follow the steps below:  

1. 	Select the desired SKUs.  
2. 	Click the <i class="fas fa-link" aria-hidden="true"></i> Link to product button.  
3. 	Enter the product ID you want to associate them with.  
4. 	Click `Approve`.  

#### Use case  

Imagine that a marketplace already has the White Shirt SKU in S, M, and L, and a seller recently submitted sizes XS and XL for the same White Shirt.  

Creating a new link groups the new sizes with the existing ones. After this, the product will have XS, S, M, L, and XL as available sizes.  

>ℹ️ This action can be applied in the offer tabs **Pending** and **Issues**.  

![received-skus-bind-to-product-en](https://images.ctfassets.net/alneenqid6w5/2fAWptfykAdJ3UTDSCpNhW/fc02d18fe2771b0603f861f8516ab7ae/received-skus-bind-to-product-en.png)

- __Link to an existing SKU:__ Creates a relationship between the new seller SKU and a SKU in the marketplace catalog. To apply this action, follow the steps below:  

1. 	Select the desired products.  
2. 	Click the <i class="fas fa-link" aria-hidden="true"></i>Link to SKU button.  
3. 	Enter the SKU ID that you want to link for each SKU you're approving.  
4. 	Click `Approve`.  

#### Use case  

A possible use case would be a marketplace that has Phone XYZ with a 128 GB memory from Seller 1.  

Now, let's say the marketplace received the same 128 GB SKU from Seller 2. To avoid duplicates in the catalog, the marketplace would have to link these two SKUs.  

>ℹ️ This action can be applied in the offer tabs **Pending** and **Issues**.

![received-skus-bind-to-sku-en](https://images.ctfassets.net/alneenqid6w5/2326FaqSqhPfQ0qeiD8KWE/8bc6c9b98e03afe02252bd69342005d1/received-skus-bind-to-sku-en.png)

- __Block:__ Blocks the selected offers. This will prevent them from being automatically processed again. To apply this action, follow the steps below:  

1. 	Select the desired products.
2. 	Click the `Reject and block` button.
3. 	Complete the __Block reason__ field. This field is optional.
4. 	Click `Reject`.  

When the marketplace blocks a SKU, it won't be included with other submitted offers the next time that the seller sends products. A SKU can be unblocked using a REST API if the marketplace wants to receive it as a suggestion from the seller. To learn more about SKU approval, see [Send SKU Suggestion](https://developers.vtex.com/docs/api-reference/marketplace-apis-suggestions#put-/suggestions/-sellerId-/-sellerSkuId-).  

>ℹ️ This action can be applied in the offer tabs **Pending** and **Issues**. Blocked offers can be viewed in the **Blocked** tab.

![received-skus-reject-and-block-en](https://images.ctfassets.net/alneenqid6w5/3rfJ5AjzArgvv7thlD3keQ/247d5dcfb554755d091b1367d84db2d5/received-skus-reject-and-block-en.png)

- __Reject for correction:__ Rejects the offer and sends an information correction request to the seller. To apply this action, follow the steps below:  

1. 	Select the desired SKUs.  
2. 	Click the __Reject for correction__ button.  
3. 	Enter the information that needs correction in the Corrections field.  
4. 	Click Reject.  

>ℹ️ This action can be applied in the offer tab **Pending**. The offers that need correction will show in the **Issues** tab.  

![received-skus-reject-for-correction-en](https://images.ctfassets.net/alneenqid6w5/62XmAvuM9luOqmLCwLpW2A/7d456cf95d5a4ed7011accdfe0550fba/received-skus-reject-for-correction-en.png)

- __Automatic approval:__ You can also set up automatic approval for SKUs from a specific seller regardless of their Matcher score. This action can only be applied through a REST API. To learn more, see [Suggestions](https://developers.vtex.com/docs/api-reference/marketplace-apis-suggestions).  
