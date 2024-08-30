---
title: 'Accounts and architecture'
id: 4yPqZQyj0t675QpcG7H6yl
status: PUBLISHED
createdAt: 2024-01-09T00:00:08.724Z
updatedAt: 2024-02-22T17:18:14.922Z
publishedAt: 2024-02-22T17:18:14.922Z
firstPublishedAt: 2024-02-22T14:06:20.581Z
contentType: trackArticle
productTeam: Others
slug: accounts-and-architecture
locale: en
trackId: eSDNk26pdvemF3XKM0nK9
trackSlugEN: vtex-store-overview
---

VTEX provides many features and products, but their availability can vary depending on the [account type](#vtex-account-types), as each one is designed for certain scenarios. Before you start planning your [store's architecture](#store-architecture) and defining [implementation partners](#implementation-partners), you need to know the main characteristics of the accounts.

## VTEX account types

The definition of a VTEX store's architecture depends on the VTEX account type, as some features are exclusive to certain account types, and each account is tailored to particular business models. The best account will be the one that best reflects the business model's structure.

VTEX account types are:

- **Main account (or standard):** The VTEX core account includes all the native settings and allows setting up a store website and requesting all platform features.
- [Franchise account](https://help.vtex.com/en/tutorial/o-que-e-conta-franquia--kWQC6RkFSCUFGgY5gSjdl): The franchise account is associated with a main account. It does not have its own website, and its most remarkable characteristic is that it does not configure its own catalog, which comes from the main account. This account type is recommended for operations with physical stores, franchisees, and brand representatives, but the store does not necessarily need to have a franchise network to benefit from the advantages of a VTEX franchise account.
- [Seller Portal account](https://help.vtex.com/en/tutorial/seller-criar-conta-no-seller-portal--3gn2Q5rMhgu0jjX7AiiHcs): This account is associated with a main account. It does not have its own website, and its main characteristic is to make the store a marketplace for [white label sellers](https://help.vtex.com/en/tutorial/seller-white-label--5orlGHyDHGAYciQ64oEgKa) or sellers outside the VTEX ecosystem who can quickly integrate their catalog in the VTEX marketplace. In other words, it is a VTEX platform edition designed for the main account's sellers.

The following image is an overview to help you [choose between standard, franchise, or Seller Portal accounts](https://help.vtex.com/en/tutorial/escolher-entre-conta-padrao-conta-franquia-ou-seller-portal--4S90HzzhMyZESsHqrnUs78):

![main_account_franchise_seller_portal_EN](https://images.ctfassets.net/alneenqid6w5/4NfyGbu9eVJFRc6EfCpTHr/b8f887b2f84c72b3c20a38a020f9c53f/main_account_franchise_seller_portal_EN.png)

## Account characteristics

[Choosing between a standard, franchise, or Seller Portal account](https://help.vtex.com/en/tutorial/escolher-entre-conta-padrao-conta-franquia-ou-seller-portal--4S90HzzhMyZESsHqrnUs78) involves many factors. The table below shows the main characteristics of each to help guide your decision:  

| **Account type** | **Main characteristics** |
| :---: | :--- |
| Main account (or standard) | <ul><li>Has its own frontend and website.</li><li>Can be multistore and have multiple sites and stores, each with its own trade policy.</li><li>Has its own VTEX Admin environment to manage its operation.</li><li>Allows you to have franchise and Seller Portal accounts and request new environments.</li><li>Allows you to natively become a <a href="https://help.vtex.com/en/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#being-a-vtex-seller">VTEX seller</a> and a <a href="https://help.vtex.com/en/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#being-a-vtex-marketplace">VTEX marketplace</a> and connect with all the stores within the VTEXecosystem.</li><li>Allows configuring <a href="https://help.vtex.com/en/tutorial/definicoes-de-conta-franquia-e-seller-white-label--5orlGHyDHGAYciQ64oEgKa">white label sellers</a> in franchise accounts.</li><li>Offers the ability to sell your franchise accounts' inventory in other VTEX marketplaces using the <a href="https://help.vtex.com/en/tutorial/multilevel-omnichannel-inventory--7M1xyCZWUyCB7PcjNtOyw4">Multilevel Omnichannel Inventory (MOI)</a> feature.</li><li>Can integrate with <a href="https://developers.vtex.com/docs/guides/external-seller-integration-guide">external sellers</a> and <a href="https://developers.vtex.com/docs/guides/external-marketplace-integration-guide">external marketplaces.</a></li><li>Allows you to request add-on products.</li></ul> |
| Franchise account | <ul><li>Does not have its own frontend or website.</li><li>Has its own VTEX Admin environment to manage its operation.</li><li>Does not have its own catalog; instead, it follows the exact catalog structure of the main account.</li><li>Allows configuring prices and promotions.</li><li>Has its own warehouse and inventory.</li><li>The franchise account inventory can be sold on other VTEX marketplaces connected to the main account via <a href="https://help.vtex.com/en/tutorial/multilevel-omnichannel-inventory--7M1xyCZWUyCB7PcjNtOyw4">Multilevel Omnichannel Inventory (MOI).</a></li></ul> |
| Seller Portal account | <ul><li>Does not have its own frontend or website.</li><li>The main account has an area for <a href="https://help.vtex.com/en/tutorial/gerenciamento-de-sellers--6eEiOISwxuAWJ8w6MtK7iv"> managing sellers</a>, and each seller has its environment in the Seller Portal Admin.</li><li>The seller can configure inventory and pricing, manage products shared with the marketplace, invoice orders, activate promotions, process payments, and have their own logistics.</li></ul> |

>ℹ️ **Marketplace on VTEX**
> Besides offering great flexibility in store architecture, our ecosystem allows each store to have multiple [marketplace strategies](https://help.vtex.com/en/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402), such as:
> *Becoming a seller or marketplace for other VTEXstores.
> * Integrating with the big players such as [Mercado Libre](https://help.vtex.com/en/tracks/configurar-integracao-do-mercado-livre--2YfvI3Jxe0CGIKoWIGQEIq) and [Amazon](https://help.vtex.com/en/tracks/configurar-integracao-com-a-amazon--6sgd4Pagy3wNsWKBvmIFrP).
>
> *Integrating with [partner marketplaces](https://help.vtex.com/en/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#integrating-with-marketplaces-partners) certified by VTEX.
>
> *Being a marketplace for sellers with a [Seller Portal](https://help.vtex.com/en/tutorial/seller-portal-primeiros-passos--6w1vBdRH2uuBGmUqgNQjwK) account.
>
> *Being a [white label seller](https://help.vtex.com/en/tutorial/seller-white-label--5orlGHyDHGAYciQ64oEgKa).
> * Creating your own integrations with [external marketplaces and external sellers.](https://developers.vtex.com/docs/guides/external-seller-integration-guide)

## Store architecture

The VTEX platform provides many business models and sizes with all the features and settings they need for your operations. For instance, a store can adopt a different strategy for each sales channel through [trade policies](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/4EPwTXx5oFdSG1dA3zIchz#trade-policy) by configuring different catalog, price, and logistics settings for each one. To do so, the only requirement is to [request new trade policies](https://help.vtex.com/en/tutorial/contratacao-de-politica-comercial-adicional--61vuFOw4yGh6nwSmkLJL1X).

However, using many trade policies simultaneously can compromise the store's performance and slow it down, as changes need to be updated across multiple trade policies. Therefore, depending on the business model and complexity of the operation, you can segment using the following options:

- [Multistores](#multistore)  
- [Additional environments](#additional-environment) 

The image below is an example of how the main account, environment (sub-account), multi-store (stores), and trade policies are related:

![multistore_aditional_environment_EN](https://images.ctfassets.net/alneenqid6w5/6XOI59M49L18E99hSDpgWe/4bf1e15428b5db24e4658c446eb5e2cf/multistore_aditional_environment_EN.png)

### Multistore

[Multistore, or multidomain](https://help.vtex.com/en/tutorial/escolhendo-entre-arquitetura-multi-loja-ou-ambiente-adicional--4HRNpa1OCKZ5YzP8yiilBL), is the feature that allows you to create other stores associated with the main account, all managed in the same admin environment. Each store will have its own [storefront](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ) and domain, but they can share module settings, such as catalog, logistics, prices, and others.

The main advantages of [creating multistores](https://help.vtex.com/en/tutorial/como-criar-multiloja-multidominio--tutorials_510) include the ease with which the company can sell different niche products, the convenience of selling multiple brands, and the agility of making different products available in different stores and channels.

The following scenarios illustrate the strategic role of having multiple stores in the same environment:

- **National and international stores:** One store is focused on the country of origin, and the other on the international market.
- **Niche segmentation:** Companies with a broad niche, operating different stores, each segmented to offer a variety of products focused on distinct audiences.
- **Different operations:** When a business operates both B2C and B2B models, for example, it can be strategic to have separate stores for each type of operation, but sharing settings and information, allowing unified management.

In addition to combining trade policies and multistores, at VTEX, you can request a new environment, as described below.

### Additional environment

A standard VTEX account can completely separate the management space for your operations by [requesting a new environment.](https://help.vtex.com/en/tutorial/contratar-novo-ambiente--tutorials_2542) Each VTEX Admin will be associated with its own account and independently manage the storefront settings and platform modules.

Some typical use cases for requesting a new environment are when you want an [environment exclusively for testing](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/6xYnNxDHUcY6FyChgziCoH#4-testing-before-the-go-live) (Quality Assurance - QA) or an environment dedicated to managing another operation, such as B2C, B2B, or B2E.

## Choosing between multistore and additional environment

The table below highlights important aspects to consider when deciding whether to have a multistore architecture, an additional environment, or a combination of both:  

| **Characteristic** | **Multistore (stores)** | **Additional environment (subaccounts)**|
| :---: | :--- | :--- |
| Architecture | A **single admin environment** in the VTEXAdmin associated with two or more stores ([store names](https://help.vtex.com/en/tutorial/o-que-e-store-name--3gh9mTNeMgs6Qe44e8IqQK)). All stores are linked to the **same [account name](https://help.vtex.com/en/tutorial/o-que-e-account-name--i0mIGLcg3QyEy8OCicEoC)**. | **Multiple admin environments** in the VTEX Admin with fully independent settings. Each environment has its own **[account name](https://help.vtex.com/en/tutorial/o-que-e-account-name--i0mIGLcg3QyEy8OCicEoC)**. |
| Sitemap | Has a single main account **[sitemap](https://help.vtex.com/en/tutorial/rastreamento-google-search-console-sitemap--tutorials_575) shared** among all stores. | Each account has its own **[sitemap](https://help.vtex.com/pt/tutorial/rastreamento-google-search-console-sitemap--tutorials_575)**. |
| Sales segmentation | Stores can **segment shopping experiences using trade policies**. This also helps ensure store performance, as you don't need multiple active trade policies. | The possibilities for sales segmentation and customization are huge, as each environment can **combine different trade policies and multistores**. |
| Team | A **single team manages the operation** or, despite different teams, the similarities in settings across stores make it more efficient for them to share catalog, logistics, and pricing settings, for example. All users are **managed by the same [License Manager](https://help.vtex.com/en/tutorial/visao-geral-do-modulo-license-manager)**. | **Different teams** within the same company have different operational responsibilities. **Each environment has its License Manager**, so [users](https://help.vtex.com/en/tutorial/gerenciando-usuarios--tutorials_512) in each of them are managed separately. |
| Costs | **There is no cost** for creating new stores, but there is a cost for creating different storefronts, as you need to [request an additional trade policy](https://help.vtex.com/en/tutorial/contratacao-de-politica-comercial-adicional--61vuFOw4yGh6nwSmkLJL1X). | **There is a cost** to [request an additional environment](https://help.vtex.com/en/tutorial/contratar-novo-ambiente--tutorials_2542?&utm_source=autocomplete), but this already includes a trade policy.|  

For more information, read the [Choosing between a multistore architecture or an additional environment](https://help.vtex.com/en/tutorial/escolhendo-entre-arquitetura-multi-loja-ou-ambiente-adicional--4HRNpa1OCKZ5YzP8yiilBL) article.

## Architecture questionnaire

To help you decide which products and settings to consider when planning your store's architecture, we've created the following table of questions:  

| **Topic** | **Questions** |
| :---: | :--- |
| Mapping existing architecture | - Are there any [external integrations](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu) to consider? For example: <br><br>- Enterprise Resource Planning (ERP) <br><br>- Customer Relationship Management (CRM) <br><br>- Transportation Management System (TMS) <br><br>- Warehouse Management System (WMS) <br><br>- Business Intelligence (BI) <br><br>- Will external integrations connect directly to the platform via [VTEX APIs](https://developers.vtex.com/docs/api-reference)? <br><br>- Will I need to request a [back office integration](https://developers.vtex.com/docs/guides/erp-integration-guide) partner? |
| How to set up a store | - Will the implementation be done using APIs from the [VTEX API Reference](https://developers.vtex.com/docs/api-reference)? <br><br>- Will the implementation be done via the VTEX Admin? <br><br>- Is it a headless commerce model that will use frontend technologies in the headless scenario? |
| [Backend](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu) and [frontend](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ) general structure | - Will I need a [partner](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/4yPqZQyj0t675QpcG7H6yl#implementation-partners) to implement the store's [backend](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu)? <br><br>- Will I need a partner to implement the [storefront](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ)? <br><br>- Is the store frontend created with any of the [VTEX technologies](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ#frontend-development-technologies-on-vtex)? ([Store Framework](https://developers.vtex.com/docs/guides/vtex-io-documentation-what-is-vtex-store-framework) and [FastStore](https://vtex.com/br-pt/resources/faststore-acelerando-a-cultura-composable-commerce-de-desenvolvimento-headless-avanti/)) <br><br>- Will the Content Management System (CMS) [storefront](https://help.vtex.com/pt/tracks/cms--2YcpgIljVaLVQYMzxQbc3z/6OCY6S9tqBXPD5mgpbBInC) in the VTEX Admin be used for store operations? <br><br>- Could the [VTEX authentication methods](https://developers.vtex.com/docs/guides/authentication) generate any friction when integrating with the VTEX platform? |
| VTEX overall structure | - Will I need [franchise accounts](https://help.vtex.com/en/tutorial/o-que-e-conta-franquia--kWQC6RkFSCUFGgY5gSjdl)? <br><br>- Should I have [white label sellers](https://help.vtex.com/em/tutorial/definicoes-de-conta-franquia-e-seller-white-label--5orlGHyDHGAYciQ64oEgKa)? <br><br>- Is it worth leveraging [Multilevel Omnichannel Inventory (MOI)](https://help.vtex.com/en/tutorial/multilevel-omnichannel-inventory--7M1xyCZWUyCB7PcjNtOyw4)? <br><br>- Will I need [Seller Portal](https://help.vtex.com/en/tutorial/seller-criar-conta-no-seller-portal--3gn2Q5rMhgu0jjX7AiiHcs) accounts? <br><br>- Will I need to request an [additional environment](https://help.vtex.com/en/tutorial/contratar-novo-ambiente--tutorials_2542)? <br><br>- Does the operation involve a [multistore/multidomain](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/4yPqZQyj0t675QpcG7H6yl#store-architecture)? <br><br>- Is it worth requesting an [additional trade policy](https://help.vtex.com/en/tracks/support-at-vtex--4AXsGdGHqExp9ZkiNq9eMy/3KQWGgkPOwbFTPfBxL7YwZ#requesting-an-additional-trade-policy)? <br><br>- Is it advisable to have a native solution to integrate with [VTEX sellers](https://help.vtex.com/en/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#being-a-vtex-seller) and [VTEX marketplaces](https://help.vtex.com/en/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#being-a-vtex-marketplace)? <br><br>- Is it advisable to integrate with [external sellers](https://developers.vtex.com/docs/guides/external-seller-integration-guide) and [external marketplaces](https://developers.vtex.com/docs/guides/external-marketplace-integration-guide)? <br><br>- What [performance optimization](https://developers.vtex.com/docs/guides/vtex-io-documentation-best-practices-for-optimizing-performance) issues should be considered in a [Store Framework development](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ#store-framework)? <br><br>- What internationalization issues should be considered in a Store Framework development? <br><br>- The operation is cross-border and needs to [manage content using bindings](https://help.vtex.com/en/tutorial/gerenciando-conteudo-por-binding--5CZjZPMqi0ZNpuqzF6AUOn) to customize the store's layout based on the users' location. |
| Industry | - What is the operation's industry? <br><br>- Is it [fashion-related](https://vtex.com/br-pt/moda-e-vestuario/) (clothes and apparel)? <br><br>- Is it [grocery-related](https://vtex.com/br-pt/supermercado/)? |
| Use cases | - Does the business model involve [B2C](https://vtex.com/br-pt/digital-commerce/) or [B2B](https://help.vtex.com/pt/tutorial/setting-up-b2b-on-vtex--tutorials_238)? <br><br>- Do I need an [omnichannel solution](https://vtex.com/br-pt/omnichannel/)? |
| [Catalog](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#catalog) | - How will the [catalog architecture](https://help.vtex.com/en/tracks/catalogo-101--5AF0XfnjfWeopIFBgs3LIQ/7kz4uWVq6NoaOdUpiJv4PR) be structured? <br><br>- Will the [catalog configuration](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu#catalog-architecture) be done via back office integration? <br><br>- Will [product import](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu#importing-products) be done via back office integration? <br><br>- Should we [internationalize the catalog](https://developers.vtex.com/docs/guides/catalog-internationalization)? |
| [Store search](https://help.vtex.com/en/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3qgT47zY08biLP3d5os3DG) | - Do I need to install and configure [VTEX Intelligent Search](https://developers.vtex.com/docs/apps/vtex.search) so customers can have an intelligent search and autocomplete function on the store's website? <br><br>- Does the operation work in multiple countries, and does it need to provide customers with [search experiences in multiple languages](https://help.vtex.com/pt/tutorial/vtex-intelligent-search-configuracoes-multi-idioma-beta--2WahlTESLXIJ9XBdQMdTYO)? <br><br>- Do you want the search results to sort the products according to a [specific merchandising rule](https://help.vtex.com/pt/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3Dvava8LSVcFKeS2S6J7XW)? <br><br>- Is it advisable to set up Region to have [seller regionalization](https://help.vtex.com/pt/tutorial/configurar-a-regionalizacao-de-sellers--32t6wLpQCEnumoh8TjT5fw)? |
| [Pricing](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#prices) and [Promotions](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#promotions) | - Considering the VTEX [pricing system architecture](https://help.vtex.com/en/tracks/precos-101--6f8pwCns3PJHqMvQSugNfP/7GptzvlPDVM11ojEjywIQx), what types of prices should be added? <br><br>- Will product pricing be configured via [back office integration](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu#prices)? <br><br>- Does the sales strategy use [price tables](https://help.vtex.com/en/tracks/precos-101--6f8pwCns3PJHqMvQSugNfP/1wAm5m3IUfIj6maBdaRJt8)? <br><br>- Do you expect to [create promotions](https://help.vtex.com/pt/tutorial/lista-de-promocoes-beta--4yB7nNdliiFxBTXE19GCIi)? |
| [Payments](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/3MYcZaojb5HSUg6ufm6GxQ#payments) | - Which gateway or set of gateways will be contacted to [add gateway affiliations to the platform](https://help.vtex.com/pt/tutorial/afiliacoes-de-gateway--tutorials_444)? <br><br>- What [payment settings](https://help.vtex.com/en/tracks/pagamentos--6GAS7ZzGAm7AGoEAwDbwJG/6bzGxlz4inf8sKmvZ1c7i3) (credit, cash, etc.) will be required for the [payment conditions](https://help.vtex.com/en/tutorial/diferenca-entre-meios-de-pagamento-e-condicoes-de-pagamento--3azJenhGFyUy2gsocms42Q) offered to customers at checkout? <br><br>- Is it advisable to set up [split payments](https://help.vtex.com/en/tutorial/split-de-pagamento--6k5JidhYRUxileNolY2VLx) for sellers and marketplaces? |
| [Logistics and fulfillment](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#logistics) | - How will the [shipping strategy](https://help.vtex.com/en/tutorial/estrategia-de-envio--58vLBDbjYVQzJ6rRc5QNz3) be structured? <br><br>- Which [loading docks](https://help.vtex.com/en/tutorial/doca--5DY8xHEjOLYDVL41Urd5qj) will be used? <br><br>- Which [warehouses](https://help.vtex.com/en/tutorial/estoque--6oIxvsVDTtGpO7y6zwhGpb) will be used? <br><br>- Which [shipping policies](https://help.vtex.com/en/tutorial/politica-de-envio--tutorials_140) will be used? <br><br>- Which [carriers](https://help.vtex.com/en/tutorial/transportadoras-na-vtex--7u9duMD5UQa2QQwukAWMcE) will be on the [shipping rate templates](https://help.vtex.com/en/tutorial/planilha-de-frete--tutorials_127) configured in the shipping policies? <br><br>- Will I need to set up [pickup points](https://help.vtex.com/en/tutorial/pontos-de-retirada--2fljn6wLjn8M4lJHA6HP3R) so customers can pick up orders from physical stores or distribution centers? <br><br>- In [inventory management](https://help.vtex.com/en/tutorial/gerenciar-itens-em-estoque--tutorials_139), is it advisable to use [lead time](https://help.vtex.com/pt/tutorial/lead_time-shipping-time-at-sku-level--16yv5Mkj6bTyWR1hCN2f4B) (an optional shipping time setting at SKU level)? <br><br>- Will [inventory import](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu#inventory) be done via back office integration? <br><br>- Is it desirable to activate the [VTEX Shipping Network Correios](https://help.vtex.com/en/tutorial/vtex-shipping-network-correios-ativacao--57opHihFbRAwrjQjCTymTa) for the operation to be integrated through the VTEX Admin with the Correios PAC and SEDEX services? (For Brazil only) <br><br>- Does the operation involve international stores and [cross-border](https://help.vtex.com/en/tracks/cms--2YcpgIljVaLVQYMzxQbc3z/5qgXy9Erm7FDP3UB5Ox8Bs) sales? |
| [Orders](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/3MYcZaojb5HSUg6ufm6GxQ#orders) | - Is it advisable to set up a [Feed or Hook](https://developers.vtex.com/docs/guides/orders-feed) to track changes in [order status](https://help.vtex.com/en/tutorial/fluxo-e-status-de-pedidos--tutorials_196)? <br><br>- Will I need a [back office integration](https://developers.vtex.com/docs/guides/erp-integration-set-up-order-integration) to send order information from VTEX to external systems such as ERP or WMS, or to send order information from external systems to VTEX? |
| [Checkout](https://help.vtex.com/en/tracks/vtex-store-overview--eSDNk26pdvemF3XKM0nK9/3MYcZaojb5HSUg6ufm6GxQ#checkout) | - Is the store going to use [VTEX Checkout](https://help.vtex.com/en/tutorial/checkout-vtex-visao-geral--7wcprkM7yZUflOqbzAN5SI) or a third-party solution? <br><br>- Is it advisable to [configure SKU pricing and availability by region](https://help.vtex.com/en/tutorial/setting-up-price-and-availability-of-skus-by-region--12ne58BmvYsYuGsimmugoc) so that the customer, in their shopping experience, sees the available store items that can be delivered to their location? |

## Implementation partners

When building a store, it is common for agencies and [implementation partners](https://vtex.com/us-en/partners/) (System Integration partners) to be involved. VTEX is associated with a wide ecosystem of partners known for their excellence and reliability in developing VTEX store projects. Provided the [user](https://help.vtex.com/en/tutorial/gerenciando-usuarios--tutorials_512) has permission to access the store's VTEX Admin, they can view the partner list on the [Partner Portal](https://partnerportal.vtex.com/) (available only in Portuguese).

The [VTEX Quadrant](https://vtex.com/pt-br/blog/parceiros/quadrante_vtex_2023/) is a program in which VTEX internally evaluates the performance and successful results of its partners' operations. This annual acknowledgment and reward is for those with the highest commitment and excellence. See the results of the 2022 Quadrant [here](https://vtex.com/pt-br/blog/parceiros/quadrante_vtex_2023/). The VTEX Quadrant is an exclusive program for implementation partners in Brazil.

>ℹ️ The [VTEX Quadrant](https://vtex.com/pt-br/blog/parceiros/quadrante_vtex_2023/) is an exclusive program for implementation partners in Brazil.