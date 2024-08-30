---
title: 'Cuentas y arquitectura'
id: 4yPqZQyj0t675QpcG7H6yl
status: PUBLISHED
createdAt: 2024-01-09T00:00:08.724Z
updatedAt: 2024-02-22T17:18:14.922Z
publishedAt: 2024-02-22T17:18:14.922Z
firstPublishedAt: 2024-02-22T14:06:20.581Z
contentType: trackArticle
productTeam: Others
slug: cuentas-y-arquitectura
locale: es
trackId: eSDNk26pdvemF3XKM0nK9
trackSlugES: serie-de-la-tienda-vtex
---

VTEX ofrece muchas funcionalidades y productos cuya disponibilidad puede variar dependiendo del [tipo de cuenta](#tipos-de-cuenta-vtex), ya que cada tipo fue creado para escenarios específicos. Antes de empezar a planificar la [arquitectura de la tienda](#arquitectura-de-la-tienda) y definir los [partners de implementación](#partners-de-implementacion), es importante conocer las principales características de las cuentas.

## Tipos de cuenta VTEX

La definición de la arquitectura de una tienda VTEX depende de la cuenta VTEX. Esto se debe a que algunas funcionalidades solo se ofrecen mediante ciertos tipos de cuenta y cada una se adapta a determinados modelos de negocio. La mejor cuenta es la que mejor refleja la estructura de ese modelo de negocio.  

Los tipos de cuenta VTEX son:

- **Cuenta principal (estándar):** es la cuenta VTEXprimordial y permite crear el sitio web de la tienda, configurar todos los ajustes nativos y contratar todos los servicios de la plataforma.
- [Cuenta franquicia](https://help.vtex.com/es/tutorial/o-que-e-conta-franquia--kWQC6RkFSCUFGgY5gSjdl): es una cuenta asociada a la cuenta principal. No tiene un sitio web propio y su característica más importante es que no permite configurar un catálogo propio, sino que lo recibe de la cuenta principal. Este tipo de cuenta se recomienda para operaciones que tienen tiendas físicas, franquicias y representantes de marca. No es obligatorio que la tienda tenga una red de franquicias para beneficiarse de los recursos de una cuenta franquicia VTEX.
- [Cuenta Seller Portal](https://help.vtex.com/es/tutorial/seller-criar-conta-no-seller-portal--3gn2Q5rMhgu0jjX7AiiHcs): es una cuenta asociada a una cuenta principal. No tiene sitio web propio y su característica más importante es que convierte la tienda en un marketplace para [sellers white label](https://help.vtex.com/es/tutorial/seller-white-label--5orlGHyDHGAYciQ64oEgKa) o sellers externos que no forman parte del ecosistema VTEXy les permite activar su propio catálogo en el marketplace VTEX. En otras palabras, es una edición de la plataforma VTEXdirigida a los sellers de la cuenta principal.  

La siguiente imagen muestra una visión general para ayudarte a [elegir entre la cuenta estándar, franquicia o Seller Portal](https://help.vtex.com/es/tutorial/escolher-entre-conta-padrao-conta-franquia-ou-seller-portal--4S90HzzhMyZESsHqrnUs78):

![main_account_franchise_seller_portal_ES](https://images.ctfassets.net/alneenqid6w5/4NfyGbu9eVJFRc6EfCpTHr/befcaed2563320ca9280d44759fe4962/main_account_franchise_seller_portal_ES.png)

## Recursos de las cuentas

Hay varios factores que se deben considerar al [elegir entre la cuenta estándar, franquicia o Seller Portal.](https://help.vtex.com/es/tutorial/escolher-entre-conta-padrao-conta-franquia-ou-seller-portal--4S90HzzhMyZESsHqrnUs78) La tabla a continuación describe los principales recursos de cada una:  

| **Tipo de cuenta** | **Características principales** |
| :---: | :--- |
| Cuenta principal (estándar) | <ul><li>Tiene frontend y sitio web propio.</li><li>Puede convertirse en <a href="https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/4yPqZQyj0t675QpcG7H6yl#multitienda">multitienda</a> y tener varios sitios web y tiendas, cada uno con su propia política comercial.</li><li>Tiene su propio entorno en el Admin VTEX para gestionar la operación.</li><li>Puede tener cuentas franquicia y Seller Portal y contratar nuevos entornos.</li><li>Permite operar como <a href="https://help.vtex.com/es/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#como-seller-vtex">seller VTEX</a> y <a href="https://help.vtex.com/es/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#ser-un-marketplace-vtex">marketplace VTEX</a> de forma nativa y conectarse con todas las tiendas del ecosistema VTEX.</li><li>Puede configurar <a href="https://help.vtex.com/es/tutorial/definicoes-de-conta-franquia-e-seller-white-label--5orlGHyDHGAYciQ64oEgKa">sellers white label</a> en cuentas franquicia.</li><li>Puede vender de forma nativa el stock de sus cuentas franquicia en otros marketplaces VTEX mediante la funcionalidad <a href="https://help.vtex.com/es/tutorial/multilevel-omnichannel-inventory--7M1xyCZWUyCB7PcjNtOyw4">Multilevel Omnichannel Inventory (MOI)</a>.</li><li>Puede integrarse con <a href="https://developers.vtex.com/docs/guides/external-seller-integration-guide">sellers externos</a> y <a href="https://developers.vtex.com/docs/guides/external-marketplace-integration-guide">marketplaces externos</a>.</li><li>Puede contratar productos add-on.</li></ul> |
| Cuenta franquicia | <ul><li>No tiene frontend ni sito web propio.</li><li>Tiene un entorno propio en el Admin VTEX para gestionar la operación.</li><li>No tiene catálogo propio y refleja la estructura de catálogo exacta de la cuenta principal.</li><li>Puede configurar precios y promociones.</li><li>Tiene almacén y stock propios.</li><li>El stock de la cuenta franquicia puede ser vendido en otros marketplaces VTEX que estén conectados con la cuenta principal a través de <a href="https://help.vtex.com/es/tutorial/multilevel-omnichannel-inventory--7M1xyCZWUyCB7PcjNtOyw4">Multilevel Omnichannel Inventory (MOI)</a>.</li></ul> |
| Cuenta Seller Portal | <ul><li>No tiene frontend ni sito web propio.</li><li>La cuenta principal tiene una página de <a href="https://help.vtex.com/es/tutorial/gerenciamento-de-sellers--6eEiOISwxuAWJ8w6MtK7iv">Gestión de sellers</a>. A su vez, cada seller cuenta un entorno independiente en el Admin del Seller Portal.</li><li>El seller puede configurar stock y precio, gestionar productos compartidos con el marketplace, facturar pedidos, activar promociones, procesar pagos y contar con logística propia.</li></ul> |  

>ℹ️ **Marketplaces en VTEX**
> Además de proporcionar gran versatilidad en la arquitectura de la tienda, nuestro ecosistema permite que cada tienda cuente con una serie de [estrategias de marketplace](https://help.vtex.com/es/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402) tales como:
> *Convertirse en seller o marketplace para otras tiendas VTEX.
> * Integrarse con importantes actores del mercado como [Mercado Libre](https://help.vtex.com/es/tracks/configurar-integracao-do-mercado-livre--2YfvI3Jxe0CGIKoWIGQEIq) y [Amazon](https://help.vtex.com/es/tracks/configurar-integracao-com-a-amazon--6sgd4Pagy3wNsWKBvmIFrP).
> * Integrarse con los [marketplaces partner](https://help.vtex.com/es/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#integrado-a-marketplaces-parceiros) certificados por VTEX.
>
> *Ser un marketplace para sellers que tengan una cuenta [Seller Portal](https://help.vtex.com/es/tutorial/seller-portal-primeiros-passos--6w1vBdRH2uuBGmUqgNQjwK).
>
> *Ser un [seller white label](https://help.vtex.com/es/tutorial/seller-white-label--5orlGHyDHGAYciQ64oEgKa).
>
> *Crear integraciones propias con [marketplaces y sellers externos](https://developers.vtex.com/docs/guides/external-seller-integration-guide).

## Arquitectura de la tienda

La plataforma VTEX ofrece a diversos modelos y tamaños de negocio todas las funcionalidades y configuraciones necesarias para sus operaciones. Por ejemplo, una tienda puede tener una estrategia diferente en cada canal de venta a través de [políticas comerciales](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/4EPwTXx5oFdSG1dA3zIchz#politicas-comerciales) y configurar un catálogo, precio y logística distinta para cada canal. Solo es necesario [contratar nuevas políticas comerciales](https://help.vtex.com/es/tutorial/contratacao-de-politica-comercial-adicional--61vuFOw4yGh6nwSmkLJL1X).

Sin embargo, el uso simultáneo de muchas políticas comerciales puede afectar el desempeño de la tienda y hacer que sea más lenta, ya que los cambios deben actualizarse en múltiples políticas. Dependiendo del modelo de negocio y la complejidad de la operación, se puede crear segmentación utilizando las siguientes opciones:  

- [Multitiendas](#multitienda)  
- [Entornos adicionales](#entorno-adicional)

La siguiente imagen es un ejemplo de la relación entre la cuenta principal, entorno (subcuenta), multitiendas (tiendas) y políticas comerciales:  

![multistore_aditional_environment_ES](https://images.ctfassets.net/alneenqid6w5/6XOI59M49L18E99hSDpgWe/a0d486cc33bba9057698b54eb2f8eaf4/multistore_aditional_environment_ES.png)

### Multitienda

[Multitienda o multidominio ](https://help.vtex.com/es/tutorial/escolhendo-entre-arquitetura-multi-loja-ou-ambiente-adicional--4HRNpa1OCKZ5YzP8yiilBL)es la funcionalidad que permite crear otras tiendas asociadas a la cuenta principal cuya gestión se llevará a cabo en el mismo entorno administrativo. Esto significa que cada tienda tendrá su propio [storefront](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ) y dominio, aunque pueden compartir la configuración de módulos, como catálogo, logística, precios, entre otros.  

Algunas de las principales ventajas de [crear multitiendas](https://help.vtex.com/es/tutorial/como-criar-multiloja-multidominio--tutorials_510) son la facilidad que le brinda a la empresa de comercializar productos con nichos diferentes, la practicidad al vender múltiples marcas y la agilidad al ofrecer diversos productos en tiendas y canales distintos.  

Los siguientes escenarios son ejemplos de casos en los que tener múltiples tiendas asociadas a un mismo entorno es estratégico:  

- **Tienda nacional e internacional:** hay una tienda para el país de origen de la operación y otra para el mercado internacional.
- **Segmentación pornicho:** se aplica a las empresas con un amplio nicho y que tienen tiendas separadas según la oferta de diferentes tipos de productos dirigidos a públicos distintos.
- **Operaciones distintas:** para los negocios que tienen operaciones B2C y B2B, por ejemplo, puede ser estratégico tener tiendas separadas para cada tipo de operación, pero que compartan muchas configuraciones e información y, así, mantener la gestión centralizada y ágil.  

Además de la combinación de políticas comerciales y multitiendas, VTEX permite contratar un nuevo entorno, como se explica a continuación.  

### Entorno adicional

Una cuenta VTEX estándar puede separar por completo el espacio de gestión de las operaciones; solo hay que [contratar un nuevo entorno](https://help.vtex.com/es/tutorial/contratar-novo-ambiente--tutorials_2542). Esto significa que cada Admin VTEX estará asociado a una cuenta propia y tendrá una configuración de storefront y módulos de la plataforma independientes.  

Algunos casos de uso comunes para contratar un nuevo entorno son cuando se quiere tener un [entorno exclusivo para pruebas](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/6xYnNxDHUcY6FyChgziCoH#4-pruebas-antes-del-go-live) (Quality Assurance - QA) o un entorno completamente separado para gestionar otra operación como B2C, B2B o B2E.

## Elegirentre multitienda y ambiente adicional

La siguiente tabla presenta los puntos importantes que se deben tomar en cuenta al decidir entre una arquitectura multitienda, entorno adicional o una combinación de ambas:

| **Tema** | **Multitienda (tiendas)** | **Entorno adicional (subcuentas)** |
| :---: | :--- | :--- |
| Arquitectura | Un __solo entorno administrativo__ en el Admin VTEX asociado a dos o más tiendas [store names](https://help.vtex.com/es/tutorial/o-que-e-store-name--3gh9mTNeMgs6Qe44e8IqQK). Todas las tiendas están vinculadas al **mismo [account name](https://help.vtex.com/es/tutorial/o-que-e-account-name--i0mIGLcg3QyEy8OCicEoC)**. | **Múltiples entornos administrativos** en el Admin VTEX con configuraciones completamente independientes. Cada entorno tiene un **[account name](https://help.vtex.com/es/tutorial/o-que-e-account-name--i0mIGLcg3QyEy8OCicEoC) propio.** |
| Mapa del sitio | Un único **[mapa del sitio](https://help.vtex.com/es/tutorial/rastreamento-google-search-console-sitemap--tutorials_575) para la cuenta principal que se comparte** entre todas las tiendas.| Cada cuenta tiene un **[mapa del sitio](https://help.vtex.com/es/tutorial/rastreamento-google-search-console-sitemap--tutorials_575) propio**. |
| Segmentación de ventas | Las tiendas pueden __segmentar experiencias de compra mediante políticas comerciales__. Esto también ayuda a mantener el desempeño de cada tienda, ya que no es necesario tener múltiples políticas comerciales activas. | Muchas posibilidades para segmentar y personalizar las ventas, ya que cada entorno puede __combinar varias políticas comerciales y multitiendas__. |
| Tipo de equipo | Un __mismo equipo gestiona__ la operación o, si hay varios equipos, la similitud en las configuraciones entre tiendas permite compartir eficientemente los ajustes de catálogo, logística y precio, entre otras. Todos los usuarios son **gestionados a través del mismo [License Manager](https://help.vtex.com/es/tutorial/visao-geral-do-modulo-license-manager)**. | __Diferentes tipos de equipos__ dentro de la empresa están encargados de distintas operaciones. __Cada entorno tiene un License Manager__ y los [usuarios](https://help.vtex.com/es/tutorial/gerenciando-usuarios--tutorials_512?&utm_source=autocomplete) de cada entorno se gestionan por separado. |
| Costos | __No hay costo__ para crear nuevas tiendas, sin embargo, para crear storefronts diferentes se requiere contratar una política comercial adicional, lo que sí conlleva un cargo. | __Hay costo__ para [contratar un entorno adicional](https://help.vtex.com/es/tutorial/contratar-novo-ambiente--tutorials_2542?&utm_source=autocomplete), pero este ya incluye una política comercial. |

Para más información, accede al artículo [Elegir entre arquitectura multitienda o entorno adicional](https://help.vtex.com/es/tutorial/escolhendo-entre-arquitetura-multi-loja-ou-ambiente-adicional--4HRNpa1OCKZ5YzP8yiilBL).

## Cuestionario sobre tipo de arquitectura

Para ayudarte a decidir qué productos y configuraciones incluir en la planificación de la arquitectura de la tienda, creamos la siguiente tabla de preguntas:

| **Tema** | **Preguntas** |
| :---: | :--- |
| Mapeo de arquitectura existente | - ¿Hay [integraciones externas](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu) que se deban considerar? Por ejemplo: <br><br> - Enterprise Resource Planning (ERP) <br><br>  - Customer Relationship Management (CRM) <br><br> - Transportation Management System (TMS) <br><br> - Warehouse Management System (WMS) <br><br> - Business Intelligence (BI) <br><br> - ¿Las integraciones externas se conectarán directamente con la plataforma utilizando las [API de VTEX](https://developers.vtex.com/docs/api-reference)? <br><br> - ¿Se requerirá contratar un [partner de integración](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/4yPqZQyj0t675QpcG7H6yl#partners-de-implementacion) para crear una [integración de back office](https://developers.vtex.com/docs/guides/erp-integration-guide)? |
| Métodos de crear la tienda | - ¿La implementación se realizará utilizando las API de [API Reference de VTEX](https://developers.vtex.com/docs/api-reference)? <br><br> - ¿La implementación se realizará a través del Admin VTEX? <br><br> - ¿Es un modelo de headless commerce que utilizará tecnologías de [frontend](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ) en el escenario headless? |
| Estructura general de [backend](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu) y [frontend](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ) | - ¿Se requerirá un partner para implementar el [backend](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/7euXDZR5CCnVFSrXyczIhu) de la tienda? <br><br> - ¿Se requerirá un partner para implementar el [frontend](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ) de la tienda? <br><br> - ¿Se creará el frontend de la tienda utilizando alguna de [las siguientes tecnologías VTEX](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/67SCtUreXxKYWhZh8n0zvZ#tecnologias-de-desarrollo-de-frontend-de-vtex)? ([Store Framework](https://developers.vtex.com/docs/guides/vtex-io-documentation-what-is-vtex-store-framework) and [FastStore](https://www.faststore.dev)) <br><br> - ¿Se utilizará el Content Management System (CMS) [Storefront](https://help.vtex.com/es/tracks/cms--2YcpgIljVaLVQYMzxQbc3z/6OCY6S9tqBXPD5mgpbBInC) en el Admin VTEX para las operaciones de la tienda? <br><br> - ¿El modelo de [autenticación](https://developers.vtex.com/docs/guides/authentication) en VTEX podría generar fricción en las integraciones con la plataforma VTEX? |
| Estructura general en VTEX | - ¿Se requerirá tener [cuentas franquicia](https://help.vtex.com/es/tutorial/o-que-e-conta-franquia--kWQC6RkFSCUFGgY5gSjdl)? <br><br> - ¿Es importante tener [sellers white label](https://help.vtex.com/es/tutorial/definicoes-de-conta-franquia-e-seller-white-label--5orlGHyDHGAYciQ64oEgKa)? <br><br> - ¿Valdría la pena aprovechar el uso de [Multilevel Omnichannel Inventory (MOI)](https://help.vtex.com/es/tutorial/multilevel-omnichannel-inventory--7M1xyCZWUyCB7PcjNtOyw4)? <br><br> - ¿Se requerirá tener cuentas [Seller Portal](https://help.vtex.com/es/tutorial/seller-criar-conta-no-seller-portal--3gn2Q5rMhgu0jjX7AiiHcs)? <br><br> - ¿Se requerirá contratar un [entorno adicional](https://help.vtex.com/es/tutorial/contratar-novo-ambiente--tutorials_2542)? <br><br>- ¿La operación usa [multitienda/multidominio](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/4yPqZQyj0t675QpcG7H6yl#arquitectura-de-la-tienda)? <br><br> - ¿Valdría contratar una [política comercial adicional](https://help.vtex.com/es/tracks/soporte-en-vtex--4AXsGdGHqExp9ZkiNq9eMy/3KQWGgkPOwbFTPfBxL7YwZ#contratacion-de-politicas-comerciales-adicionales)? <br><br> - ¿Sería conveniente tener la solución nativa para crear integraciones con [sellers VTEX](https://help.vtex.com/es/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#como-seller-vtex) y [marketplaces VTEX](https://help.vtex.com/es/tutorial/estrategias-de-marketplace-na-vtex--tutorials_402#ser-un-marketplace-vtex)? <br><br> - ¿Sería conveniente crear integraciones con [sellers externos](https://developers.vtex.com/docs/guides/external-seller-integration-guide) y [marketplaces externos](https://developers.vtex.com/docs/guides/external-marketplace-integration-guide)? <br><br> - ¿Qué puntos de [optimización de rendimiento](https://developers.vtex.com/docs/guides/vtex-io-documentation-best-practices-for-optimizing-performance) deben tomarse en cuenta en el desarrollo en Store Framework? <br><br> - ¿Qué puntos de internacionalización deben tomarse en cuenta en el desarrollo en Store Framework? <br><br> - La operación es internacional y requiere [gestionar contenido mediante binding](https://help.vtex.com/es/tutorial/gerenciando-conteudo-por-binding--5CZjZPMqi0ZNpuqzF6AUOn) para personalizar la apariencia de la tienda según la ubicación de los usuarios. |
| Tipo de sector | - ¿Cuál es el sector de la operación? <br><br> - ¿Está relacionado con [moda](https://vtex.com/mx-es/moda-y-vestuario/) (ropa y vestuario)? <br><br> - ¿Está relacionado con [supermercado](https://vtex.com/mx-es/supermercado/)?  |
| Caso de uso | - ¿El modelo de negocio incluye [comercio B2C](https://vtex.com/ar-es/digital-commerce/) o [comercio B2B](https://help.vtex.com/es/tutorial/setting-up-b2b-on-vtex--tutorials_238)? <br><br> - ¿Se requerirá una [solución omnichannel](https://vtex.com/co-es/omnichannel/)? |
| [Catálogo](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#catalogo) | - ¿Cuál será la [arquitectura del catálogo](https://help.vtex.com/es/tracks/catalogo-1015AF0XfnjfWeopIFBgs3LIQ/7kz4uWVq6NoaOdUpiJv4PR) de productos? <br><br> - ¿La integración back office realizará la configuración del catálogo? <br><br> - ¿Se importarán los productos a través de una [integración de back office](https://developers.vtex.com/docs/guides/erp-integration-import-products)? <br><br> - ¿Hay que [internacionalizar el catálogo](https://developers.vtex.com/docs/guides/catalog-internationalization)? |
| [Búsquedas en el sitio web de la tienda](https://help.vtex.com/es/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3qgT47zY08biLP3d5os3DG) | - ¿Hay que instalar y configurar [VTEX Intelligent Search](https://developers.vtex.com/docs/apps/vtex.search) para que los clientes dispongan de búsqueda inteligente y autocompletar en el sitio web de la tienda? <br><br> - ¿La operación está presente en varios países y necesita ofrecer una experiencia de [búsqueda en múltiples idiomas](https://help.vtex.com/es/tutorial/vtex-intelligent-search-configuracoes-multi-idioma-beta--2WahlTESLXIJ9XBdQMdTYO) a los clientes? <br><br> - ¿Deseas que la tienda ordene los productos en los resultados de búsqueda siguiendo alguna [regla de merchandising específica](https://help.vtex.com/es/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/3Dvava8LSVcFKeS2S6J7XW)? <br><br> - ¿Sería beneficioso configurar Region para [regionalizar a los sellers](https://help.vtex.com/es/tutorial/configurar-a-regionalizacao-de-sellers--32t6wLpQCEnumoh8TjT5fw)? |
| [Precios](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#precios) y [Promociones](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#promociones) | - ¿Considerando la [arquitectura del sistema de precios](https://help.vtex.com/es/tracks/precos-101--6f8pwCns3PJHqMvQSugNfP/7GptzvlPDVM11ojEjywIQx) en VTEX, qué tipos de precios se registrarán? <br><br> - ¿Se configurarán los precios de los productos a través de una integración de back office? <br><br> - ¿La estrategia de ventas utiliza [tablas de precios](https://help.vtex.com/es/tracks/precos-101--6f8pwCns3PJHqMvQSugNfP/1wAm5m3IUfIj6maBdaRJt8)? <br><br> - ¿Se espera [crear promociones](https://help.vtex.com/es/tutorial/lista-de-promocoes-beta--4yB7nNdliiFxBTXE19GCIi)? |
| [Pagos](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/3MYcZaojb5HSUg6ufm6GxQ#pagos) | - ¿Con qué gateway o grupo de gateways habrá contacto para después [registrar las afiliaciones de gateway](https://help.vtex.com/es/tutorial/afiliacoes-de-gateway--tutorials_444) en la plataforma? <br><br> - ¿Qué [configuraciones de pago](https://help.vtex.com/es/tracks/pagamentos--6GAS7ZzGAm7AGoEAwDbwJG/6bzGxlz4inf8sKmvZ1c7i3) (crédito, efectivo, etc.) se requerirán para las [condiciones de pago](https://help.vtex.com/es/tutorial/diferenca-entre-meios-de-pagamento-e-condicoes-de-pagamento--3azJenhGFyUy2gsocms42Q) ofrecidas a los clientes en el checkout? <br><br> - ¿Sería conveniente configurar el [split de pagos](https://help.vtex.com/es/tutorial/split-de-pagamento--6k5JidhYRUxileNolY2VLx) para sellers y marketplaces? |
| [Logística y fulfillment](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/75MX4aorniD0BYAB8Nwbo7#logistica) | - ¿Cómo se organizará la [estrategia de envío](https://help.vtex.com/es/tutorial/estrategia-de-envio--58vLBDbjYVQzJ6rRc5QNz3)? <br><br> - ¿Cuáles serán los [muelles](https://help.vtex.com/es/tutorial/doca--5DY8xHEjOLYDVL41Urd5qj)? <br><br> - ¿Cuáles serán los [almacenes](https://help.vtex.com/es/tutorial/estoque--6oIxvsVDTtGpO7y6zwhGpb)? <br><br> - ¿Cuáles serán las [políticas de envío](https://help.vtex.com/es/tutorial/politica-de-envio--tutorials_140)? <br><br> - ¿Qué [transportadoras](https://help.vtex.com/es/tutorial/transportadoras-na-vtex--7u9duMD5UQa2QQwukAWMcE) de las [plantillas de envío](https://help.vtex.com/pt/tutorial/planilha-de-frete--tutorials_127) se configurarán en las políticas de envío? <br><br> - ¿Se configurarán [puntos de recogida](https://help.vtex.com/es/tutorial/pontos-de-retirada--2fljn6wLjn8M4lJHA6HP3R) para que los clientes puedan recoger los pedidos en tiendas físicas o centros de distribución? <br><br> - ¿En la [gestión de stock](https://help.vtex.com/es/tutorial/gerenciar-itens-em-estoque--tutorials_139) sería conveniente configurar el [lead time](https://help.vtex.com/es/tutorial/lead_time-shipping-time-at-sku-level--16yv5Mkj6bTyWR1hCN2f4B) (ajuste opcional de tiempo de envío a nivel de SKU)?<br><br> - ¿Se importará el stock a través de una integración de back office? <br><br> - ¿Sería conveniente activar [VTEX Shipping Network Correios](https://help.vtex.com/es/tutorial/vtex-shipping-network-correios-ativacao--57opHihFbRAwrjQjCTymTa) para integrar la operación con los servicios de PAC y SEDEX de Correios a través del Admin? (Solo Brasil). <br><br> - ¿La operación tiene tiendas internacionales y ventas [cross border](https://help.vtex.com/es/tracks/cms--2YcpgIljVaLVQYMzxQbc3z/5qgXy9Erm7FDP3UB5Ox8Bs)? |
| [Pedidos](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/3MYcZaojb5HSUg6ufm6GxQ#pedidos) | - ¿Sería conveniente configurar [Feed o Hook](https://developers.vtex.com/docs/guides/orders-feed) para monitorear los cambios de [status de los pedidos](https://help.vtex.com/es/tutorial/fluxo-e-status-de-pedidos--tutorials_196)? <br><br> - ¿Se requerirá una [integración de back office](https://developers.vtex.com/docs/guides/erp-integration-set-up-order-integration) para enviar los datos de pedidos VTEX a sistemas externos como ERP o WMS, o para enviar datos de pedidos de sistemas externos a VTEX? |
| [Checkout](https://help.vtex.com/es/tracks/serie-de-la-tienda-vtex--eSDNk26pdvemF3XKM0nK9/3MYcZaojb5HSUg6ufm6GxQ#checkout) | - ¿La tienda utilizará [VTEX Checkout VTEX](https://help.vtex.com/es/tutorial/checkout-vtex-visao-geral--7wcprkM7yZUflOqbzAN5SI) o una solución externa? <br><br> - ¿Sería conveniente [configurar el precio y disponibilidad de SKU a nivel regional](https://help.vtex.com/es/tutorial/setting-up-price-and-availability-of-skus-by-region--12ne58BmvYsYuGsimmugoc) de modo que el cliente vea primero los ítems de la tienda con stock en su ubicación? |

## Partners de implementación

Es común que agencias y [partners de implementación ](https://vtex.com/mx-es/partner/)(system integration partners) participen de la creación de una tienda. VTEX se asocia con un amplio ecosistema de partners que han sido reconocidos por su excelencia y confiabilidad al crear proyectos de tiendas VTEX. Siempre que el [usuario](https://help.vtex.com/es/tutorial/gerenciando-usuarios--tutorials_512) tenga permiso de acceso al Admin VTEX de una tienda, puede consultar la lista de partners a través del [Partner Portal](https://partnerportal.vtex.com/) (solamente en portugués).

El [Cuadrante VTEX](https://vtex.com/pt-br/blog/parceiros/quadrante_vtex_2023/) es un programa en que VTEX evalúa internamente el rendimiento y los resultados de éxito de operación de sus partners. Es una forma de reconocer y recompensar anualmente a los partners que demuestren el máximo nivel de entrega y excelencia. [Aquí](https://vtex.com/pt-br/blog/parceiros/quadrante_vtex_2023/) puedes ver el resultado del Cuadrante VTEX 2023.

>ℹ️ El [Cuadrante VTEX](https://vtex.com/pt-br/blog/parceiros/quadrante_vtex_2023/) es un programa exclusivo para partners de implementación en Brasil.
