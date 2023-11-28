---
title: '[!UICONTROL Security] &gt; [!UICONTROL Google reCAPTCHA Storefront]'
description: Revise as configurações no [!UICONTROL Security] &gt; [!UICONTROL Google reCAPTCHA Storefront] página do Administrador do Commerce.
exl-id: 6c03ee68-7421-4c74-bdc1-0855f088b7f9
feature: Configuration, Security
source-git-commit: 76bd1b1af9b55d69bd98209d70fb5518f190a3e1
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 0%

---

# [!UICONTROL Security] > [!UICONTROL Google reCAPTCHA Storefront]

>[!IMPORTANT]
>
>Antes que o Google reCAPTCHA possa ser configurado, você deve garantir que seu `PHP.ini` O arquivo inclui a seguinte configuração: `allow_url_fopen = 1`. Isso pode exigir ajuda do desenvolvedor. Consulte [Configurações do PHP](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) no _Guia de instalação_.

{{config}}

Para obter mais informações sobre como usar o Google reCAPTCHA para proteger sua loja, consulte Google [reCAPTCHA](../../systems/security-google-recaptcha.md) no _Guia de sistemas do administrador_.

## [!UICONTROL reCAPTCHA v2 ("I am not a robot")]

![reCAPTCHA v2 (&quot;Não sou um robô&quot;)](./assets/recaptcha-storefront-v2-not-robot.png)<!-- zoom -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--|--|--|
| [!UICONTROL Google API Website Key] | Site | A chave do site que é criada ao registrar sua conta do Google reCAPTCHA. |
| [!UICONTROL Google API Secret Key] | Site | A chave secreta associada à sua conta do Google reCAPTCHA. |
| [!UICONTROL Size] | Site | O tamanho da caixa do Google reCAPTCHA que aparece quando um cliente faz logon em sua conta. Opções: `Normal` (padrão) / `Compact` |
| [!UICONTROL Theme] | Site | Determina o estilo da caixa do reCAPTCHA do Google. Opções: `Light Theme` (padrão) / `Dark Theme` |
| [!UICONTROL Language Code] | Exibição de loja | A variável [código de dois caracteres](https://developers.google.com/recaptcha/docs/language) que especifica o idioma usado para mensagens e texto do Google reCAPTCHA. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL reCAPTCHA v2 Invisible]

![reCAPTCHA v2 Invisível](./assets/recaptcha-storefront-v2-invisible.png)<!-- zoom -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--|--|--|
| [!UICONTROL Google API Website Key] | Site | A chave do site que é criada ao registrar sua conta do Google reCAPTCHA. |
| [!UICONTROL Google API Secret Key] | Site | A chave secreta associada à sua conta do Google reCAPTCHA. |
| [!UICONTROL Invisible Badge Position] | Site | A posição do selo reCAPTCHA invisível em cada página. Opções: `Inline` / `Bottom Right` / `Bottom Left` |
| [!UICONTROL Theme] | Global | Determina o estilo da caixa do reCAPTCHA do Google. Opções: `Light Theme` (padrão) / `Dark Theme` |
| [!UICONTROL Language Code] | Exibição de loja | A [código de dois caracteres](https://developers.google.com/recaptcha/docs/language) que especifica o idioma usado para mensagens e texto do Google reCAPTCHA. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL reCAPTCHA v3 Invisible]

![reCAPTCHA v3 Invisível](./assets/recaptcha-storefront-v3-invisible.png)<!-- zoom -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--|--|--|
| [!UICONTROL Google API Website Key] | Site | A chave do site que é criada ao registrar sua conta do Google reCAPTCHA. |
| [!UICONTROL Google API Secret Key] | Site | A chave secreta associada à sua conta do Google reCAPTCHA. |
| [!UICONTROL Minimum Score Threshold] | Global | A pontuação mínima que identifica uma interação do usuário como um risco potencial, onde 1,0 é uma interação típica do usuário e 0,0 provavelmente é um bot. Padrão: `0.5` |
| [!UICONTROL Invisible Badge Position] | Site | A posição do selo reCAPTCHA invisível em cada página. Opções: `Inline` / `Bottom Right` / `Bottom Left` |
| [!UICONTROL Theme] | Site | Determina o estilo da caixa do reCAPTCHA do Google. Opções: `Light Theme` (padrão) / `Dark Theme` |
| [!UICONTROL Language Code] | Exibição de loja | A [código de dois caracteres](https://developers.google.com/recaptcha/docs/language) que especifica o idioma usado para mensagens e texto do Google reCAPTCHA. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL reCAPTCHA Failure Messages]

![Mensagens de falha](./assets/recaptcha-storefront-failure-messages.png)<!-- zoom -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--|--|--|
| [!UICONTROL reCAPTCHA Validation Failure Message] | Exibição de loja | A mensagem que é exibida na loja se a verificação falhar. Texto padrão: `reCAPTCHA verification failed.` |
| [!UICONTROL reCAPTCHA Technical Failure Message] | Exibição de loja | A mensagem exibida na loja se o reCAPTCHA não retornar um resultado de verificação. Texto padrão: `Something went wrong with reCAPTCHA. Please contact the store owner.` |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Storefront]

![Loja](./assets/recaptcha-storefront.png)<!-- zoom -->

>[!NOTE]
>
>O tipo do reCAPTCHA escolhido deve corresponder ao tipo associado à chave de API da sua conta do Google reCAPTCHA.

>[!WARNING]
>
>Ao usar o reCAPTCHA versão 3, um usuário genuíno com baixa pontuação não pode continuar. Para a versão 2, um usuário genuíno com uma pontuação baixa recebe um desafio. Considere cuidadosamente se os usuários originais com uma pontuação baixa devem ter a oportunidade de resolver um desafio (versão 2) ou ser bloqueados (versão 3).

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--|--|--|
| [!UICONTROL Enable for Customer Login] | Site | Especifica o tipo de reCAPTCHA que é usado quando os clientes [fazer logon](../../customers/customer-sign-in.md) às suas contas. Opções:<br/>**`No`**- (padrão) Não valida a solicitação de logon.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Forgot Password] | Site | Especifica o tipo de reCAPTCHA que é usado quando os clientes solicitam uma [redefinição de senha](../../customers/password-reset.md). Opções:<br/>**`No`**- (padrão) Não valida a solicitação de redefinição de senha.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Create New Customer Account] | Site | Especifica o tipo de reCAPTCHA que é usado quando o cliente se inscreve em um [nova conta](../../customers/account-create.md). Opções:<br/>**`No`**- (padrão) Não valida a solicitação de conta.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Edit Customer Account] | Site | Especifica o tipo de reCAPTCHA que é usado quando o cliente altera seus [informações da conta](../../customers/account-dashboard-account-information.md). Opções:<br/>**`No`**- (padrão) Não valida a solicitação de conta.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Create New Company Account] | Site | ![B2B para Adobe Commerce](../../assets/b2b.svg) (Disponível com B2B somente para Adobe Commerce) Especifica o tipo de reCAPTCHA que é usado quando um novo [conta da empresa](../../b2b/account-company-create.md) é criado. Opções:<br/>**`No`**- (padrão) Não valida a solicitação de conta.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Contact Us] | Site | Especifica o tipo de reCAPTCHA usado para enviar uma mensagem do [Entre em contato](../../getting-started/store-details.md#contact-us-form) página da sua loja. Opções:<br/>**`No`**- (padrão) Não valida a solicitação de mensagem.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Product Review] | Site | Especifica o tipo de reCAPTCHA que é usado quando os clientes enviam um [análise do produto](../../merchandising-promotions/product-reviews.md). Opções:<br/>**`No`**- (padrão) Não valida a solicitação de revisão do produto.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Newsletter Subscription] | Site | Especifica o tipo de reCAPTCHA invisível que é usado quando os clientes se inscrevem para um [assinatura do informativo](../../merchandising-promotions/newsletter-subscribers.md). Opções:<br/>**`No`**- (padrão) Não valida a solicitação de assinatura do boletim informativo.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Gift Card] | Site | ![Adobe Commerce](../../assets/adobe-logo.svg) (Somente Adobe Commerce) Especifica o tipo de reCAPTCHA que é usado quando os clientes inserem uma [cartão-presente](../../catalog/product-gift-card-create.md) código. Opções:<br/>**`No`**- (padrão) Não valida o envio do código do cartão-presente.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Invitation Create Account] | Site | Especifica o tipo de reCAPTCHA usado quando os clientes enviam uma criação de conta [convite](../../merchandising-promotions/invitations.md) código. Opções:<br/>**`No`**- (padrão) Não valida o envio do email de convite.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Send to Friend] | Site | Especifica o tipo de reCAPTCHA que é usado quando os clientes [compartilhar um produto](../../stores-purchase/email-a-friend.md) com um amigo. Opções:<br/>**`No`**- (padrão) Não valida o envio de email.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Wishlist Sharing] | Site | Especifica o tipo de reCAPTCHA que é usado quando os clientes [compartilhar uma lista de desejos](../../stores-purchase/wishlist-storefront.md#share-the-wish-list). Opções:<br/>**`No`**- (padrão) Não valida a mensagem e o envio de email.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for Coupon Codes] | Site | Especifica o tipo de reCAPTCHA que é usado quando os clientes inserem um [código do cupom](../../merchandising-promotions/price-rules-cart-coupon.md). Opções:<br/>**`No`**- (padrão) Não valida o envio do código do cupom.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |
| [!UICONTROL Enable for PayPal Payflow Pro payment form] | Site | Especifica o tipo de reCAPTCHA usado quando os clientes pagam uma compra com [PayPal Payflow Pro](../../stores-purchase/paypal-payflow-pro.md). Opções:<br/>**`No`**- (padrão) Não valida a solicitação de redefinição de senha.<br />**`reCAPTCHA v2 ("I am not a robot")`** - Exige que o usuário selecione o _Eu não sou um robô_ caixa de seleção <br />**`Invisible reCAPTCHA v2`**- Valida o comportamento do usuário em segundo plano sem exigir interações com base na pontuação.<br/>**`Invisible reCAPTCHA v3`** - (Recomendado) Valida o comportamento do usuário em segundo plano com base na pontuação de interação. |

{:style=&quot;table-layout:auto&quot;}