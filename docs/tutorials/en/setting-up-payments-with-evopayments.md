---
title: 'Setting up payments with EvoPayments'
id: 7CxSgoftps0DHsfR8otQMf
status: PUBLISHED
createdAt: 2024-03-11T17:36:12.910Z
updatedAt: 2024-03-14T16:37:46.611Z
publishedAt: 2024-03-14T16:37:46.611Z
firstPublishedAt: 2024-03-11T18:19:00.757Z
contentType: tutorial
productTeam: Financial
author: 6DODK49lJPk3yvcoe6GB6g
slug: setting-up-payments-with-evopayments
locale: en
legacySlug: setting-up-payments-with-evopayments
subcategory: 3tDGibM2tqMyqIyukqmmMw
---

At VTEX, it is possible to integrate with the EVO Payments payment provider. With this provider, your store can make sales through credit, debit, private labels and cobranded cards, and bank invoices.

To configure EVO Payments, follow the steps below:

1. In the VTEX Admin, go to __Store Settings > Payment > Providers__, or type __Providers__ in the search bar at the top of the page.
2. On the providers screen, click the `New Provider` button.
3. Type the name __EvoPayments__ in the search bar and click on the name of the provider.
4. In __Provider Authorization__, fill in the __App Key__ and __App token__ fields with data provided by EVO Payments.
5. If you wish to modify the identification name to be displayed for the EVO Payments provider on the VTEX Admin screen, enter the information in the __Name__ field in __Basic Information__.
6. In __Payment Control__, select whether you want to activate the provider in a test environment by clicking __Enable test mode__.
7. In the __Automatic settlement__ field, select one of the following option:
<br>
<ul>
<br>
    	<li><b>Use behavior recommended by the payment processor</b>: Capture is not automatic; it is scheduled according to the period specified by the acquirer. The acquirer indicates whether the payment has been authorized and can determine or recommend a number of days for the capture upon payment authorization. (This is the platform's default behavior).</li>
    	<li><b>Automatic capture immediately after payment authorization</b>: Capture is automatically performed right after payment authorization, even if the transaction includes an anti-fraud analysis.</li>
   		<li><b>Automatic capture immediately after anti-fraud analysis</b>: Capture is automatically performed right after payment authorization and anti-fraud analysis. If you select this behavior and do not have anti-fraud analysis, the system will perform the payment capture as in "Automatic capture immediately after payment authorization".</li>     
   		<li><b>Disabled</b>: Capture takes place only when the order is invoiced. If you select this behavior, it is important to pay attention to the invoicing time, as invoicing can exceed the capture time agreed with the payment provider and lead to the cancellation of the transaction.</li>
</ul>
8. In __Habilitar autenticación 3DS__, select whether you want to enable 3DS security validation.
9. In __Habilitar autorización y captura__, select whether you want to activate this function.
10. In __Habilitar plan Iphone For Life__, select whether you want to activate this option. 
11. Click `Save`.

To configure the payment methods to be processed by EVO Payments, access [Configuring Payment Conditions](https://help.vtex.com/en/tutorial/how-to-configure-payment-conditions--tutorials_455#).

To set special conditions on payment methods, go to [Configuring payment special conditions](https://help.vtex.com/en/tutorial/special-conditions--tutorials_456#).

After following the indicated steps, EVO Payments may take up to 10 minutes to appear at your store's checkout as a payment option.