---
title: 'SKUs recebidos'
id: 4hxDUmbgOEVFSTU2Eqi8DK
status: PUBLISHED
createdAt: 2024-04-29T13:48:12.818Z
updatedAt: 2024-06-25T19:27:37.735Z
publishedAt: 2024-06-25T19:27:37.735Z
firstPublishedAt: 2024-04-29T14:16:25.091Z
contentType: tutorial
productTeam: Channels
author: 2p7evLfTcDrhc5qtrzbLWD
slug: skus-recebidos-beta
locale: es
legacySlug: anuncios-recebidos
subcategory: 
---

La página SKUs recibidos permite al [marketplace](https://help.vtex.com/es/tutorial/visao-geral-marketplace--40Zd0z9h2RXsM9uMUp3kEb) ver, priorizar y catalogar los ítems enviados por sus sellers. Esto posibilita la creación de nuevos productos y su asociación con SKU o productos ya existentes para ponerlos a disposición para la venta. Accede a la página a través del Admin VTEX en __Marketplace > SKUs recibidos__  o ingresa __SKUs recibidos__ en la barra de búsqueda del Admin.  

La catalogación puede realizarse de forma manual o automática, [mediante uno o varios matchers](https://help.vtex.com/es/tutorial/entendendo-a-pontuacao-do-vtex-matcher?locale=pt), y también mediante [autoApprove](https://developers.vtex.com/docs/api-reference/marketplace-apis-suggestions/#put-/suggestions/configuration/autoapproval/toggle). También existe la posibilidad de utilizar herramientas externas para realizar esta operación.  

En este artículo encontrarás una visión general sobre la [Estructura de la página](#estructura-de-la-pagina), [Priorizar la catalogación](#priorizar-la-catalogacion) y [Catalogación de ítems](#catalogacion-de-items).  

## Estructura de la página

La página SKUs recibidos se organiza en pestañas correspondientes a los distintos status posibles de un anuncio:  

- [Pendientes](#pendientes)  
- [Problemas](#problemas)  
- [Aprobados](#aprobados)  
- [Procesando](#procesando)  
- [Bloqueados](#bloqueados)  

Dentro de cada pestaña, además de visualizar la lista de SKU, es posible filtrar anuncios, revisar las especificaciones de cada uno y verificar el porcentaje de SKUs recibidos que se encuentran en ese status específico.  

![skus-recibidos-pestanas-es](https://images.ctfassets.net/alneenqid6w5/4jNrRvJsZgja1LuSz204P1/3757c1f533031f535b2c233eb55f3d08/skus-recibidos-pestanas-es.png)

### Pendientes

En la pestaña __Pendientes__, el marketplace puede consultar la lista de todos los anuncios enviados por un seller y que aún no han sido aprobados. Los anuncios se pueden filtrar por __seller, categoría, marca y stock.__ También pueden llevarse a cabo las siguientes acciones en anuncios de esta pestaña: __Crear nuevo producto, Asociar con producto o SKU, Rechazar para corrección o Rechazar y bloquear.__

Cada fila de la lista representa un producto con la siguiente información:  

- __Anuncio:__ muestra el nombre del producto.  
- __ID del SKU:__ número que identifica el producto.  
- __Seller:__ nombre del seller que envió el anuncio.  
- __Categoría:__ categoría en la que el producto está registrado, si ya se realizó el mapeo. Si el mapeo de categoría aún no se ha realizado, se mostrará el mensaje No mapeada.  
- __Precio:__ precio del producto enviado por el seller.  
- __Stock:__ cantidad disponible de ese producto.  

Para consultar todas las especificaciones de un producto, haz clic en el nombre del producto deseado y se abrirá una nueva ventana con toda la información.  

![skus-recibidos-analisis-es](https://images.ctfassets.net/alneenqid6w5/3QSXyYXqhdAB3R4J3lL749/d789b0d0ad6be43a7eb75ee0b6a0c637/skus-recibidos-analisis-es.png)

### Problemas

En la pestaña __Problemas__ están disponibles todos los anuncios que aún no se aprobaron debido a problemas que requieren corrección por parte del seller. Los filtros, acciones y campos de identificación disponibles en la pestaña **[Pendientes](#pendientes)** son similares a los de la pestaña Problemas.  

>ℹ️ La acción de solicitar corrección no está disponible en la pestaña **Problemas.**  

Para identificar el problema de un anuncio solo hay que hacer clic en el nombre del producto deseado. Se mostrará una nueva ventana con la información del producto, el mensaje de error y el revisor del anuncio.  

![skus-recibidos-problemas-analisis-es](https://images.ctfassets.net/alneenqid6w5/4yZtOcq16r6SXvai0lWzau/9209d4817cfdb057283cb12a6bdb99a6/skus-recibidos-problemas-analisis-es.png)

### Aprobados

En la pestaña __Aprobados__ se muestran los SKUs recibidos y aprobados. En esta pestaña puedes __Editar el producto, Ver la página del producto__ y __filtrar anuncios por seller, categoría y marca.__

Cada fila de la lista representa un producto con la siguiente información:   

- __Anuncio:__ muestra el nombre del producto.  
- __ID del SKU:__ número que identifica el producto.  
- __Seller:__ nombre del seller que envió el anuncio.  
- __Categoría:__ indica la categoría a la que pertenece el producto.  

### Procesando  

En la pestaña __Procesando__ se encuentran los SKUs recibidos que están siendo evaluados por el sistema VTEX.  En esta pestaña solo se puede visualizar la información, con opciones de filtros por __seller__ y __fecha de envío__ del producto.  

Cada fila de la lista representa un producto con la siguiente información:  

- __Anuncio:__ muestra el nombre del producto.  
- __ID de SKU:__ número que identifica el producto.  
- __Seller:__ nombre del seller que envió el anuncio.  
- __Fecha de envío:__ muestra la fecha en que se envió el anuncio al marketplace.  

>ℹ️ Los anuncios aquí listados están siendo evaluados por Matcher y por Offer Quality o autoApprove, en caso de que se hayan configurado. Tras la evaluación, el anuncio puede pasar a las pestañas **Pendientes, Problemas, Aprobados o Bloqueados**, dependiendo del cumplimiento de los requisitos establecidos.  

### Bloqueados

En la pestaña __Bloqueados__ pueden consultarse los anuncios enviados por el seller que han sido bloqueados por el marketplace. En esta pestaña puedes __desbloquear__ un anuncio y también filtrar anuncios por __seller__ y __revisor.__

Cada fila de la lista representa un producto con la siguiente información:  

- __Anuncio:__ muestra el nombre del producto.  
- __ID del SKU:__ número que identifica el producto.  
- __Seller:__ nombre del seller que envió el anuncio.  
- __Revisor:__ nombre del agente que realiza la revisión del anuncio.  

## Priorizar la catalogación 

La lista de SKUs recibidos se ha desarrollado para priorizar y agilizar la catalogación de los ítems que la componen. Al hacer clic en cualquier SKU de la lista, accedes a un resumen de la información principal del SKU por medio de una barra lateral, sin salir de la página del listado. En la barra lateral también se muestra el porcentaje de match asignado al SKU por el matcher instalado en tu tienda.  

Algunas de las funcionalidades que ayudan en el proceso de priorización son:  

### Filtros  

En cada una de las pestañas presentadas en la sección anterior es posible combinar diferentes filtros para configurar la visualización deseada de SKU.  

Por ejemplo, si se selecciona la marca ABC y la categoría Medias, en la vista se mostrarán todos los SKU de la marca ABC que pertenezcan a la categoría Medias.  

Cabe señalar que las opciones de filtros se basan en los SKU disponibles en la lista. Ejemplo: un marketplace está conectado a los sellers A, B y C, pero solo existen SKU pendientes de los sellers B y C. Esto significa que la selección del filtro en la pestaña [Pendientes](#pendientes) solo mostrará los resultados de los sellers B y C.  

### Orden  

De manera predeterminada, los ítems más recientemente agregados se muestran primero en la lista. Sin embargo, el orden también puede determinarse por __Precio__ y __Stock.__   

En este caso, los ítems se ordenarán de forma ascendente o descendente al hacer clic en __Precio__ o __Stock.__

![skus-recibidos-ord-es](https://images.ctfassets.net/alneenqid6w5/3Eur3cPCdSTtZjoGIqeq6o/a44da25a3176f26b0ab2e318ef171375/skus-recibidos-ord-es.png)

## Catalogación de ítems  

Todos los SKU que se muestran en la lista ya están disponibles para catalogación. No obstante, se recomienda realizar el [mapeo de categorías y marcas](https://help.vtex.com/es/tutorial/mapeamento-de-categorias-e-marcas-para-marketplace-vtex-beta--6NU8LwR6i0tTb8nk30bnbE) antes de este paso para agilizar el proceso de catalogación.  

>⚠️ Los anuncios de la pestaña Pendientes permanecen disponibles solamente durante 30 días. Pasado este periodo, expiran automáticamente y el seller tendrá que volver a enviarlos.

### Opciones de catalogación  

Para catalogar un anuncio, accede a la página __SKUs recibidos__ en el Admin VTEX haciendo clic en __Marketplace > SKUs recibidos__ o ingresando __SKUs recibidos__ en la barra de búsqueda del Admin.  
>ℹ️ Todos los anuncios de la pestaña Pendientes se pueden catalogar individualmente o en masa.

Las acciones disponibles para la catalogación son:  

- __Crear nuevo producto:__ crea un nuevo SKU en el catálogo, lo que a su vez crea un nuevo producto. Recomendamos utilizar esta opción cuando un determinado producto aún no existe en el catálogo del marketplace. Para llevar a cabo esta acción, sigue los pasos a continuación:

1. Selecciona los SKU deseados.  
2. Haz clic en el botón <i class="fas fa-plus" aria-hidden="true"></i> `Crear nuevo producto`.  
3. Completa los campos __Categoría__ y __Marca__ para cada producto. Si el mapeo ya se ha realizado previamente, estos campos ya estarán completados.  
4. Haz clic en `Aprobar`.  

>ℹ️ Esta acción puede realizarse en las pestañas **Pendientes** y **Problemas**.

![skus-recibidos-crear-nuevo-producto-es](https://images.ctfassets.net/alneenqid6w5/4H2vmekbrtbXQXUVrwVoSF/4b686bea24c2df091c8739ecc398a645/skus-recibidos-crear-nuevo-producto-es.png)

- __Asociar a un producto existente:__ crea una relación entre el producto del seller y un producto que ya existe en el catálogo del marketplace. Para llevar a cabo esta acción, sigue los pasos a continuación:  

1. Selecciona los SKU deseados.  
2. Haz clic en el botón <i class="fas fa-link" aria-hidden="true"></i> `Asociar al producto`.  
3. Ingresa el ID del producto al que se asociará.  
4. Haz clic en `Aprobar`.  

#### Caso de uso  

Imagina el siguiente escenario: el marketplace ya tiene el SKU Camisa blanca en las tallas S, M y L. Pero recientemente, el seller ha agregado al stock las tallas XS y XL del mismo producto, Camisa blanca.  

Al crear una nueva asociación, las nuevas tallas se agrupan con las demás que ya estaban previamente registradas. Por lo tanto, el producto estará disponible en las tallas XS, S, M, L y XL.  

>ℹ️ Esta acción puede realizarse en las pestañas **Pendientes** y **Problemas**.

![skus-recibidos-vincular-al-producto-es](https://images.ctfassets.net/alneenqid6w5/2fAWptfykAdJ3UTDSCpNhW/7bf8dee7e2b09fa4c36aefa485a461c8/skus-recibidos-vincular-al-producto-es.png)

- __Asociar a un SKU existente:__ crea una relación entre el SKU del seller y un SKU que ya existe en el catálogo del marketplace. Para llevar a cabo esta acción, sigue los pasos a continuación:  

1. Selecciona los productos deseados.  
2. Haz clic en el botón <i class="fas fa-link" aria-hidden="true"></i> Asociar al SKU.  
3. Ingresa el ID del SKU que se asociará a cada SKU que se está aprobando.  
4. Haz clic en Aprobar.  

#### Caso de uso  

Imagina el siguiente escenario: un marketplace tiene el smartphone XYZ con 128 GB de memoria del Seller 1.  

No obstante, es posible que este marketplace reciba el mismo SKU de 128 GB del Seller 2. Para evitar duplicar el catálogo, el marketplace debe asociar estos SKU.  

<div class="alert-info">
Esta acción puede realizarse en las pestañas <b>Pendientes</b> y <b>Problemas</b>.
</div>

![skus-recibidos-vincular-al-sku-es](https://images.ctfassets.net/alneenqid6w5/2326FaqSqhPfQ0qeiD8KWE/5d8fc3e9ba0d93b2c2f9186d73f4f69b/skus-recibidos-vincular-al-sku-es.png)

- __Bloquear:__ esta acción bloquea los anuncios seleccionados, impidiendo su reprocesamiento automático. Para llevar a cabo esta acción, sigue los pasos a continuación:  

1. Selecciona los productos deseados.  
2. Haz clic en el botón `Rechazar y bloquear `.  
3. Rellena el campo __Motivo del bloqueo__ (opcional). O preenchimento é opcional.  
4. Haz clic en `Rechazar`.  

Cuando el marketplace bloquea un SKU, significa que la próxima vez que el seller envíe sus productos, aquellos que hayan sido bloqueados ya no serán incluidos entre los enviados. Es posible desbloquear un SKU a través de la API REST, si el marketplace desea volver a recibirlo como sugerencia del seller. Para más información sobre la aprobación de SKU, consulta nuestra documentación [Send SKU Suggestion](https://developers.vtex.com/docs/api-reference/marketplace-apis-suggestions#put-/suggestions/-sellerId-/-sellerSkuId-).  

>ℹ️ Esta acción puede realizarse en las pestañas **Pendientes** y **Problemas**. Los anuncios bloqueados se mostrarán en la pestaña **Bloqueados**.

![skus-recibidos-rechazar-y-bloquear-es](https://images.ctfassets.net/alneenqid6w5/3rfJ5AjzArgvv7thlD3keQ/bb22e0cfd4ff98513d5da66696b2e5d5/skus-recibidos-rechazar-y-bloquear-es.png)

- Rechazar para corrección: rechaza el anuncio y envía al seller una solicitud para corregir la información. Para llevar a cabo esta acción, sigue los pasos a continuación:  

1. Selecciona los SKU deseados.  
2. Haz clic en el botón `Rechazar para corrección`.  
3. Completa el campo __Correcciones__ con la información que el seller debe corregir.  
4. Haz clic en `Rechazar`.  

>ℹ️ Esta acción puede realizarse en la pestaña **Pendientes**. Los anuncios que necesitan corrección se mostrarán en la pestaña **Problemas**.  

![skus-recibidos-rechazar-para-correccion-es](https://images.ctfassets.net/alneenqid6w5/62XmAvuM9luOqmLCwLpW2A/bc526e9f64a729781f5ebebcd6a62ee0/skus-recibidos-rechazar-para-correccion-es.png)

- __Aprobación automática:__ también puedes configurar la aprobación automática de SKU de un seller específico, independientemente de la puntuación asignada por Matcher. Esta acción solo puede realizarse a través de la API REST. Para saber más, consulta la documentación de [Suggestions](https://developers.vtex.com/docs/api-reference/marketplace-apis-suggestions).  