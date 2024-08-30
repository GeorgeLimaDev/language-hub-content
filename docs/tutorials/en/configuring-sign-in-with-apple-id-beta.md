---
title: 'Configuring Sign in with Apple ID (Beta)'
id: 5qprgEmHYfPTghnYwm0KrV
status: PUBLISHED
createdAt: 2023-09-05T17:38:23.553Z
updatedAt: 2023-09-05T18:22:20.252Z
publishedAt: 2023-09-05T18:22:20.252Z
firstPublishedAt: 2023-09-05T18:22:20.252Z
contentType: tutorial
productTeam: Identity
author: 1malnhMX0vPThsaJaZMYm2
slug: configuring-sign-in-with-apple-id-beta
locale: en
legacySlug: configuring-sign-in-with-apple-id-beta
subcategory: 5uXA9a0laSLMkfbv6jQRDS
---

>ℹ️ This feature is in closed beta, which means that only specific customers can access it now. If you want to implement it in the future, please contact [our support](https://support.vtex.com/hc/en-us/).

On VTEX, customers don't need to create an account or log in to make a purchase. However, if they want to change the information provided during their first purchase, they must prove the email belongs to them.

The platform natively allows logging in with email and password or using an access code sent to the customer's email. We also offer optional native integrations with Apple ID, [Google, and Facebook](https://help.vtex.com/en/tutorial/configuring-login-with-facebook-and-google--tutorials_513), which need to be configured. This guide explains the required configuration to enable Sign in with [Apple ID](https://support.apple.com/apple-id) in your store:

- [Prerequisites](#prerequisites)
- [Registering on Apple](#registering-on-apple)
- [Completing the authentication information](#completing-the-authentication-information)
- [Testing Sign in with Apple ID](#testing-sign-in-with-apple-id)
- [Limitations](#limitations)

## Prerequisites

Before configuring Sign in with Apple ID for your store, you need to have an[ Apple ID](https://support.apple.com/apple-id) and be enrolled in the [Apple Developer Program](https://developer.apple.com/programs/).

## Registering on Apple

To configure the login integration with Apple, you must create OAuth 2.0 credentials (the protocol used for integration) in this service. To do so, follow the instructions in our [Registering credentials to set up Apple ID login](https://developers.vtex.com/docs/guides/registering-credentials-to-set-up-apple-id-login) developer guide.

## Completing the authentication information

Once you have registered with Apple, enable the option of logging in to your store using this provider by following the instructions below. Make sure you have the credentials provided in the registration step.

1. In the top bar of the VTEX Admin, click **your profile avatar**, indicated by the initial letter of your email address.
2. Click **Account settings > Authentication**.

    You will be redirected to the **Webstore** tab of the **Authentication** page, which lists the login methods available in your store.

1. In the **Apple** row, click `Set Up`.
2. Complete the configuration fields with the [credentials previously registered on Apple](#registering-on-apple):

    - **Key ID:** Identifier of the private key generated by Apple that VTEX will use to generate the [OAuth client secret](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/).
    - **Team ID:** Identifier of your team on the [Apple Developer Portal](https://developer.apple.com/).
    - **Service ID:** Identifier of your Apple service, which will be used as the [OAuth `client_id`](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/).
    - **P8 Certificate:** Private key saved as a text file with a `.p8` file extension generated only once by Apple when creating the key.

    Check out the [Registering credentials to set up Apple ID login](https://developers.vtex.com/docs/guides/registering-credentials-to-set-up-apple-id-login) developer guide to learn how to get these credentials.

    ![apple-id-setup-en](https://images.ctfassets.net/alneenqid6w5/3llgZRzP1yyUiqgZjagXyT/aa8a24c6942c41dc122db4172e6730f6/apple-id-setup-en.png)

5. Click `Save`.
6. Click `Webstore Providers` to go back to the previous page.
7. Click the _switch_ <i class="fas fa-toggle-on"></i> to enable Apple as the login provider.

## Testing Sign in with Apple ID

Once everything is configured, you can test it. We recommend that you test the configuration with the final URL through which users will access your store. The Apple ID option should be available when you try to log in.

1. Go to your store's website and click `Sign In`.
2. Click `Sign in with Apple`. You will be taken to the Apple login window.
3. Enter your Apple ID and password.
4. Complete the two-factor authentication if requested.
5. Choose whether to share your email with the app or [hide it](https://support.apple.com/en-us/HT210425) and click `Continue`. We recommend sharing the email, as there are [limitations](#limitations) with hidden email on VTEX.

>ℹ️ The option of whether to share your email appears only when you first access the store with your Apple ID. After that, you only need to click `Continue`. To reset the email sharing option, visit [Apple ID management](https://appleid.apple.com/us/), revoke your store authorization, and log in again.

By doing so, you will be logged in to the store.

## Limitations

Please consider the current limitations on logging in with Apple ID in VTEX stores:

- Message Center is not compatible with Apple emails, so emails configured in the tool will not be sent to users who log in with an Apple ID.
- If the user chooses to use Apple's [Hide My Email](https://support.apple.com/en-us/HT210425) feature, VTEX will generate a new account every time the user logs in.

   This means that if someone initially logs in with an email and password, places an order, and later logs in using Apple ID with the hidden email feature enabled, VTEX will create a separate account. This new account will not be associated with the original account and will not allow access to order history or other user information. This action cannot be undone.