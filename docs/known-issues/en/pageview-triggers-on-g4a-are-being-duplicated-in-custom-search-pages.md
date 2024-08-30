---
title: 'Pageview triggers on G4A are being duplicated in custom search pages'
id: 4hIwZ2v9bbyyZXrxoDglyx
status: PUBLISHED
createdAt: 2023-11-08T13:35:27.802Z
updatedAt: 2024-02-19T18:43:16.271Z
publishedAt: 2024-02-19T18:43:16.271Z
firstPublishedAt: 2023-11-08T13:35:28.390Z
contentType: knownIssue
productTeam: Store Framework
author: 2mXZkbi0oi061KicTExNjo
tag: Store Framework
slug: pageview-triggers-on-g4a-are-being-duplicated-in-custom-search-pages
locale: en
kiStatus: Backlog
internalReference: 888042
---

## Summary


The pageView event is showing duplicated in dataLayer when on custom search pages


##

## Simulation



- Go to any custom search page
- Open your browser's console
- Type dataLayer and check the pageView event

The expected behavior is the duplicated event


##

## Workaround


N/A


## **Internal Notes**

Also found something curious on department page with pageView and page_view

https://storetheme.vtex.com/apparel---accessories/

 ![](https://vtexhelp.zendesk.com/attachments/token/dXFuDY5Q9XhZ7hgIvA8m8ugJ3/?name=image.png)

But, this specific issue is replicable at

https://www.dzarm.com.br/outlet

 ![](https://vtexhelp.zendesk.com/attachments/token/EVakZYSBKtcrCQoNXBe92uAzQ/?name=image.png)
