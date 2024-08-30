---
title: 'SKU Selector with multilpe contexts'
id: 4n6ap30jnJOrzflLCnVziO
status: PUBLISHED
createdAt: 2024-01-29T13:31:21.812Z
updatedAt: 2024-07-11T19:19:22.383Z
publishedAt: 2024-07-11T19:19:22.383Z
firstPublishedAt: 2024-01-29T13:31:22.391Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: sku-selector-with-multilpe-contexts
locale: en
kiStatus: Fixed
internalReference: 341322
---

## Summary



SKU selector inside modal/quick view is not in the same context that is in the search page and product page.

 ![](https://vtexhelp.zendesk.com/attachments/token/zIQ15WW7s1Zo24Z1I5tFT4H3y/?name=image.png)


 ![](https://vtexhelp.zendesk.com/attachments/token/gnAeV75W2Sip3Pl1zfQyAiWOI/?name=image.png)


##

## Simulation



- Go to any store that has a quick view and sku-selector.
- Pick an SKU and go to the quick view mode
- Change the SKU inside the quick view modal
- Exit quick view mode and you will notice that the sku didn't change, it just changed inside the quick view context


##

## Workaround


N/A
