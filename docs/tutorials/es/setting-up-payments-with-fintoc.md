---
title: 'Configurar pago con Fintoc'
id: 3TIz2oxbNtzhypWiypqrOZ
status: PUBLISHED
createdAt: 2023-07-14T17:06:16.055Z
updatedAt: 2024-01-24T17:39:34.960Z
publishedAt: 2024-01-24T17:39:34.960Z
firstPublishedAt: 2023-07-14T17:49:20.115Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: configurar-pago-con-fintoc
locale: es
legacySlug: configurar-pago-con-fintoc
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

En VTEX es posible la integración con el proveedor de pagos Fintoc. Con este proveedor, su tienda puede realizar ventas a través de Fintoc.

Para configurar Fintoc, siga los pasos a continuación:

1. En el Admin VTEX, accede a __Configuración de la tienda > Pago > Proveedores__, o escribe __Proveedores__ en la barra de búsqueda en la parte superior de la página.
2. En la pantalla de proveedores, haga clic en el botón `Nuevo proveedor`.
3. Escriba el nombre __Fintoc__ en la barra de búsqueda y haga clic en el nombre del proveedor.
4. Rellene los campos de registro __Application Key__, __Application Token__ y __Secret Key__ con los datos proporcionados por su cuenta Fintoc.
5. Si aparece un mensaje de alerta que indica la necesidad de instalar la aplicación, haga clic en el botón `Instalar aplicación` y siga las instrucciones de instalación.
6. Haga clic en `Guardar`.

## Configurar condición de pago
1. En el Admin VTEX, accede a __Configuración de la tienda > Pago > Configuración__, o escribe __Configuración__ en la barra de búsqueda en la parte superior de la página.
2. En la pestana __Condiciones de pago__, haga clic en el botón __+__.
3. Haga clic en __Fintoc__.
4. Active la condición en el campo __Status__.
5. Si desea utilizar un sistema antifraude, seleccione la opción __Utilizar antifraude__.
6. Si desea, puede [configurar condiciones especiales de pago](https://help.vtex.com/es/tutorial/condiciones-especiales--tutorials_456?&utm_source=autocomplete#).
7. Haga clic en `Guardar`.

Después de seguir los pasos indicados, Fintoc puede tardar hasta 10 minutos en aparecer en el checkout de tu tienda como una opción de pago.