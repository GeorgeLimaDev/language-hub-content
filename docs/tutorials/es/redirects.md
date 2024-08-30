---
title: 'Redireccionamientos'
id: 3okF84cImJwKzcc8hxmZ2r
status: PUBLISHED
createdAt: 2024-06-27T17:04:44.975Z
updatedAt: 2024-06-27T17:05:31.676Z
publishedAt: 2024-06-27T17:05:31.676Z
firstPublishedAt: 2024-06-27T17:05:31.676Z
contentType: tutorial
productTeam: Marketing & Merchandising
author: 2o8pvz6z9hvxvhSoKAiZzg
slug: redireccionamientos
locale: es
legacySlug: redireccionamientos
subcategory: 1wvyJwJhKgewxGeAGCVmM6
---

La funcionalidad de **Redireccionamientos** direcciona al cliente a cualquier otra página, ya sea interna o externa a la tienda. Los redireccionamientos se hacen en el área de búsqueda de tu storefront, utilizando términos o filtros que el cliente haya seleccionado. De este modo, una de las ventajas de los redireccionamientos es contemplar escenarios de comunicación que la búsqueda en el catálogo de la tienda no cubre, como por ejemplo redirigir la búsqueda de una marca a su página promocional.

>⚠️ Esta funcionalidad está disponible en VTEX Intelligent Search Multidioma. Lee nuestro artículo VTEX Intelligent Search: configuración Multidioma (Beta) para obtener más información.

## Cómo funciona un redireccionamiento

Al crear un redireccionamiento, también es necesario crear condiciones - llamadas reglas. Estas deben contener un conjunto tanto de términos como de filtros registrados. La cantidad de reglas es ilimitada por redireccionamiento.

Mediante la funcionalidad de Redireccionamientos se pueden crear reglas que contemplen los intereses del gestor y del cliente final simultáneamente. Otros beneficios son:

- Aumentar las posibilidades de búsqueda del sitio. Las búsquedas sin resultados generan estadísticamente Tasa de Rechazo (Bounce Rate) - el porcentaje de visitantes que entran en el sitio y salen sin ver otras páginas - para el comercio electrónico.
- Facilitar la usabilidad del cliente final, como en situaciones de poscompra o en acciones promocionales.

Después de que el cliente haya realizado una búsqueda, VTEX Intelligent Search captura el término de búsqueda y comprueba si hay alguna regla de redireccionamiento registrada relacionada con esta búsqueda.

El término de búsqueda es elegible cuando ya existe, por lo menos, una regla relacionada con este. Así, el cliente es redireccionado a la URL registrada.

Puedes crear un redireccionamiento que, si el cliente busca “Mis pedidos” o “Pedidos”, lo dirija a los pedidos de la cuenta en lugar de ver una página de búsqueda vacía.

Además, también puedes configurar la funcionalidad para dirigir al cliente a una landing page de promociones específicas. En este caso, el cliente que busque "Black Friday" será dirigido a esta promoción.

En otro escenario, si el cliente busca "Zapatilla de correr" y filtra la marca Nike, será llevado a una página específica de la marca.
