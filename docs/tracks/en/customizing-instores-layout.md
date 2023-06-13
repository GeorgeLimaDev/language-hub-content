---
title: Customizing inStore's layout
id: 7Hsd9UGwZeqPeAGs2k80BH
status: DRAFT
createdAt: 2020-06-28T19:17:52.655Z
updatedAt: 2021-11-25T14:00:41.141Z
publishedAt: 
firstPublishedAt: 2020-06-28T19:22:31.049Z
contentType: trackArticle
productTeam: Shopping
slug: customizing-instores-layout
trackId: 1z9kBm12oBPyVNDo1ivVc2
trackSlugEN: customizing-instores-layout
---

<div class="alert alert-danger">
Customizing the inStore layout, as explained in this article, involves changing the CSS file <code>checkout-instore-custom.css</code>. This operation should only be performed by people with programming experience. Incorrect changes to this file can cause critical errors.
</div>

Through the VTEX administrative panel, the store has access to the editable CSS file that defines the styles of the inStore app. Therefore, it is possible to customize these styles.

The file that must be changed is exclusively `checkout-instore-custom.css`.

It is located in the Checkout settings, within the Admin of your VTEX store.

To access this file directly, you can enter the following URL in your browser: `https://{{AccountName}}.myvtex.com/admin/portal#/sites/default/code/files/checkout-instore-custom.js`

In this case, `{{AccountName}}` should be replaced with your VTEX store account name.

After editing the file's CSS rules, be sure to save it.
