---
title: Diacritics are removed on CatalogAPI
id: 2iVyAQ8TSaT3jFYzcQGjSs
status: PUBLISHED
createdAt: 2022-07-22T18:18:04.236Z
updatedAt: 2022-11-25T21:44:21.525Z
publishedAt: 2022-11-25T21:44:21.525Z
firstPublishedAt: 2022-07-22T18:18:05.160Z
contentType: knownIssue
productTeam: Catalog
author: 2mXZkbi0oi061KicTExNjo
tag: Catalog
slug: diacritics-are-removed-on-catalogapi
kiStatus: Backlog
internalReference: 623345
---

## Summary



Currently, some diacritic characters, such as ă are not preserved when saved using the catalogAPI: https://developers.vtex.com/vtex-rest-api/reference/catalog-api-put-product





## Simulation


1 - use a put product API https://developers.vtex.com/vtex-rest-api/reference/catalog-api-put-product with a diacritic
Ex:
 ![](https://vtexhelp.zendesk.com/attachments/token/DZhYXsOPhCpPGWfd7LikCfnCq/?name=image.png)

2 - Then either check this data via API or catalog admin, you'll have these characters removed: https://developers.vtex.com/vtex-rest-api/reference/catalog-api-get-product

 ![](https://vtexhelp.zendesk.com/attachments/token/zac0UZAZFzPR9unBs7EtqsdxR/?name=image.png)





## Workaround


Manually update these products via admin UI

