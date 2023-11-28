---
title: '[!UICONTROL Customers]  &gt; [!UICONTROL Customer Configuration]'
description: Revise as configurações no [!UICONTROL Customers] &gt; [!UICONTROL Customer Configuration] página do Administrador do Commerce.
exl-id: 596359d7-3891-4e0c-9604-3647032188fd
feature: Configuration, Customers
source-git-commit: 76bd1b1af9b55d69bd98209d70fb5518f190a3e1
workflow-type: tm+mt
source-wordcount: '1898'
ht-degree: 0%

---

# [!UICONTROL Customers]  > [!UICONTROL Customer Configuration]

{{config}}

## [!UICONTROL Account Sharing Options]

![Opções de compartilhamento de conta](./assets/customer-configuration-account-sharing-options.png)<!-- zoom -->

<!-- [Account Sharing Options](https://docs.magento.com/user-guide/customers/account-scope.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Share Customer Accounts] | Global | Determina o escopo das contas do cliente na hierarquia da loja. Opções: <br/>**`Global`**- As informações da conta do cliente são compartilhadas com todos os sites e armazenadas na instalação do Commerce.<br/>**`Per Website`** - As informações de conta do cliente estão limitadas ao site onde a conta foi criada. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Online Customers Options]

![Opções de clientes on-line](./assets/customer-configuration-online-customers-options.png)<!-- zoom -->

<!-- [Online Customers Options](https://docs.magento.com/user-guide/customers/now-online.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Online Minutes Interval] | Global | Determina o período de tempo em que a atividade online de um cliente pode ser acessada pelo Administrador. Deixe vazio por um intervalo padrão de 15 minutos. |
| [!UICONTROL Customer Data Lifetime] | Global | Determina o número de minutos antes que os dados não salvos inseridos pelo cliente expirem. Por padrão, os dados não salvos expiram após 60 minutos. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Create New Account Options]

{{beta-updates}}

![Criar novas opções de conta](./assets/customer-configuration-create-new-account-options.png)<!-- zoom -->

![Criar novas opções de conta (campos de IVA)](./assets/customer-configuration-create-new-account-options-vat.png)<!-- zoom -->

<!-- [Create New Account Options (VAT Fields)](https://docs.magento.com/user-guide/customers/customer-account-configuration.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Enable Automatic Assignment to Customer Group] | Exibição da loja | Determina se os clientes são atribuídos automaticamente ao grupo de clientes padrão. Para mostrar o número IVA na loja, defina Mostrar número IVA na vitrine, selecione `Yes`. Opções: <br/>**`Yes`**- O sistema não valida automaticamente as IDs de IVA do cliente nem altera os grupos de clientes.<br/>**`No`** - O comportamento do sistema é o habitual e o grupo de clientes padrão pode ser definido no campo Grupo Padrão. |
| [!UICONTROL Default Group] | Exibição da loja | Identifica o grupo de clientes inicial atribuído quando uma conta é criada. |
| [!UICONTROL Default Value for Disable Automatic Group Changes Based on VAT ID] | Global | (Disponível somente se o escopo da configuração atual estiver definido como `Default Group`.) Escolha se a alteração automática do grupo de clientes com base na ID de IVA está habilitada ou desabilitada por padrão. A configuração pode ser substituída no nível do produto. A configuração influencia o comportamento do sistema nas seguintes situações: <br/> - A ID de IVA do endereço padrão do cliente ou todo o endereço padrão é alterado. <br/> - A alteração de grupo de clientes foi emulada durante o check-out para um cliente registrado que não tinha nenhum endereço salvo anteriormente ou para um cliente que se registrou durante o check-out. <br/>Se a alteração automática do grupo estiver habilitada, no primeiro caso, o grupo de clientes será alterado automaticamente e, no segundo caso, o grupo de clientes emulado temporariamente será atribuído ao cliente. Se a alteração automática de grupo estiver desativada, o grupo de clientes atribuído nunca será alterado, a menos que um administrador altere-o manualmente. |
| [!UICONTROL Show VAT Number on Storefront] | Site | Determina se o número de IVA é visível para clientes no armazenamento. Opções: `Yes` / `No` <br/> Afeta somente as contas de clientes não B2B comuns. As contas da empresa têm seu próprio campo de Número IVA separado. |
| [!UICONTROL Default Email Domain] | Exibição da loja | Identifica o domínio de email padrão da loja. Por exemplo: `mystore.com` |
| [!UICONTROL Default Welcome Email] | Exibição da loja | Identifica o modelo de email usado para o padrão _Bem-vindo_ email. |
| [!UICONTROL Default Welcome Email Without Password] | Exibição da loja | Um modelo alternativo de email de boas-vindas usado para novas contas de clientes criadas pelo Administrador que ainda não têm uma senha atribuída. |
| [!UICONTROL Email Sender] | Exibição da loja | Identifica o contato de armazenamento que aparece como remetente do email de boas-vindas. |
| [!UICONTROL Require Emails Confirmation] | Site | Determina se uma solicitação para criar uma conta requer a confirmação do cliente. Opções: `Yes` / `No` |
| [!UICONTROL Confirmation Link Email] | Exibição da loja | Identifica o modelo de email usado para o email de confirmação. Modelo padrão: `New account confirmation key` |
| [!UICONTROL Welcome Email] | Exibição da loja | Identifica o modelo de email usado para a mensagem de boas-vindas enviada depois que a conta é confirmada. |
| [!UICONTROL Generate Human-Friendly Customer ID] | Global | Determina se o campo usado para inserir e armazenar o número da ID de IVA está visível na loja. Opções: `Yes` / `No` |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Password Options]

![Opções de senha](./assets/customer-configuration-password-options.png)<!-- zoom -->

<!-- [Password Options](https://docs.magento.com/user-guide/customers/password-options.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Password Reset Protection Type] | Exibição da loja | Determina o método usado para redefinir a senha de uma conta de cliente. Opções: <br/>**`By IP and Email`**- A senha pode ser redefinida online depois que uma resposta é recebida de uma notificação de redefinição enviada para o endereço de email associado à conta de Administrador.<br/>**`By IP`** - A senha pode ser redefinida online. <br/>**`By Email`**- A senha pode ser redefinida respondendo a uma notificação por email enviada para o endereço de email associado à conta de Administrador.<br/>**`None`** - A senha pode ser redefinida somente pelo administrador da loja. |
| [!UICONTROL Max Number of Password Reset Requests] | Exibição da loja | Limita o número de solicitações de redefinição de senha por hora. Para solicitações ilimitadas, insira zero (0). |
| [!UICONTROL Min Time Between Password Reset Requests] | Exibição da loja | Determina o número de minutos entre as solicitações de redefinição de senha. Para que não haja atraso entre as solicitações, digite zero (0). |
| [!UICONTROL Forgot Email Template] | Exibição da loja | Identifica o template de email usado quando os clientes esquecem suas senhas. Modelo padrão: `Forgot Password` |
| [!UICONTROL Remind Email Template] | Exibição da loja | Identifica o modelo de email usado quando os clientes recebem um lembrete de senha ou uma dica. Modelo padrão: `Remind Password` |
| [!UICONTROL Reset Password Template] | Exibição da loja | Determina o modelo de email usado quando os clientes redefinem suas senhas. |
| [!UICONTROL Password Template Email Sender] | Exibição da loja | Determina o contato da loja que aparece como o remetente de emails relacionados a senhas. |
| [!UICONTROL Recovery Link Expiration Period (hours)] | Global | Especifica o número de horas antes de um link de recuperação de senha expirar. |
| [!UICONTROL Enable Autocomplete on login/forgot password forms] | Site | Determina se o preenchimento automático está ativado nos formulários de login/senha esquecida. Opções: `Yes` / `No` |
| [!UICONTROL Number of Required Character Classes] | Global | Determina o número de classes de caracteres diferentes (minúsculas, maiúsculas, numéricas e caracteres especiais) que devem ser incluídas em uma senha. |
| [!UICONTROL Maximum Login Failures to Lockout Account] | Global | Determina o número de tentativas de login com falha até que a conta do cliente seja bloqueada. Para tentativas ilimitadas, digite zero (`0`). |
| [!UICONTROL Minimum Password Length] | Global | Determina o número mínimo de caracteres permitidos em uma senha. O número deve ser maior que zero (`0`). |
| [!UICONTROL Lockout Time (minutes)] | Global | Determina por quantos minutos uma conta do cliente será bloqueada após muitas tentativas de logon com falha. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Account Information Options]

![Opções de informações da conta](./assets/customer-configuration-account-info-options.png)<!-- zoom -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Change Email Template] | Exibição da loja | Identifica o modelo de email padrão usado quando um cliente altera seu endereço de email. |
| [!UICONTROL Change Email and Password Template] | Exibição da loja | Identifica o modelo de email padrão que é usado quando um cliente altera seu endereço de email e senha. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Name and Address Options]

### opções de Magento Open Source

{{ce-feature}}

![Opções de Nome e Endereço - Abrir Origem](./assets/customer-configuration-name-address-options-ce.png)<!-- zoom -->

<!-- [Name and Address Options - Open Source](https://docs.magento.com/user-guide/customers/name-address-options.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Number of Lines in a Street Address] | Site | Determina o número de linhas no endereço. O endereço consiste em de `1` para `4` linhas. Se o campo estiver em branco, o endereço padrão será três (`3`) é usada. |
| [!UICONTROL Show Prefix] | Site | Determina se o nome do cliente inclui um prefixo no início, como Sr. e Sra. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Prefix Dropdown Options] | Site | Define a lista de opções de prefixo. Separe os valores com um ponto e vírgula. Coloque um ponto e vírgula antes do primeiro valor para exibir um valor vazio na parte superior da lista. |
| [!UICONTROL Show Middle Name (initial)] | Site | Determina se a inicial do meio está incluída como parte do nome do cliente. Se usado, a inicial do meio é um campo opcional. Opções: `Yes` / `No` |
| [!UICONTROL Show Suffix] | Site | Determina se o nome do cliente inclui um sufixo no final, como Jr., Sr. e III. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Suffix Dropdown Options] | Site | Define a lista de opções de sufixo. Separe os valores com um ponto e vírgula. Coloque um ponto e vírgula antes do primeiro valor para exibir um valor vazio na parte superior da lista. |
| [!UICONTROL Show Date of Birth] | Site | Determina se a data de nascimento do cliente está incluída no formulário de nome e endereço. Opções: `No` / `Optional` / `Required`  <br><br>**_Importante:_**De acordo com as práticas recomendadas atuais de segurança e privacidade, esteja ciente de possíveis riscos legais e de segurança associados ao armazenamento da data de nascimento completa do cliente (mês, dia, ano) com outros identificadores pessoais. É recomendável limitar o armazenamento das datas de nascimento completas dos clientes e sugerir o uso do ano de nascimento do cliente como alternativa. |
| [!UICONTROL Show Tax/VAT Number] | Site | Determina se o Imposto ou [Número de IVA](../../stores-purchase/vat.md) está incluído no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Show Gender] | Site | Determina se o gênero está incluído no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Show Telephone] | Site | Determina se o número de telefone do cliente está incluído no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Show Company] | Site | Determina se a empresa do cliente está incluída no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Show Fax] | Site | Determina se o número de fax do cliente está incluído no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |

{:style=&quot;table-layout:auto&quot;}

### Opções do Adobe Commerce

{{ee-feature}}

![Opções de nome e endereço - Comércio](./assets/customer-configuration-name-address-options-ee.png)<!-- zoom -->

<!-- [Name and Address Options - Commerce](https://docs.magento.com/user-guide/customers/name-address-options.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Prefix Dropdown Options] | Site | Define a lista de opções de prefixo. Separe os valores com um ponto e vírgula. Coloque um ponto e vírgula antes do primeiro valor para exibir um valor vazio na parte superior da lista. |
| [!UICONTROL Suffix Dropdown Options] | Site | Define a lista de opções de sufixo. Separe os valores com um ponto e vírgula. Coloque um ponto e vírgula antes do primeiro valor para exibir um valor vazio na parte superior da lista. |
| [!UICONTROL Show Telephone] | Site | Determina se o número de telefone do cliente está incluído no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Show Company] | Site | Determina se a empresa do cliente está incluída no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |
| [!UICONTROL Show Fax] | Site | Determina se o número de fax do cliente está incluído no formulário de nome e endereço. Opções: `No` / `Optional` / `Required` |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Store Credit Options]

{{ee-feature}}

![Opções de Crédito da Loja](./assets/customer-configuration-store-credit-options.png)<!-- zoom -->

<!-- [Store Credit Options](https://docs.magento.com/user-guide/customers/credit-configure.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Enable Store Credit Functionality] | Global | Determina se o Crédito da Loja está habilitado. Desativá-la remove o Crédito da Loja das contas do cliente e da página Gerenciar clientes do administrador. Opções: `Yes` / `No`. |
| [!UICONTROL Show Store Credit History to Customers] | Site | Determina se o histórico de saldo está visível nas contas do cliente. Opções: `Yes` / `No`. |
| [!UICONTROL Refund Store Credit Automatically] | Global | Determina se o reembolso de armazenamento é emitido automaticamente. Opções: `Yes` / `No` |
| [!UICONTROL Store Credit Update Email Sender] | Exibição da loja | Determina a identidade da loja que aparece como o remetente das notificações de atualização de crédito enviadas aos clientes. |
| [!UICONTROL Store Credit Update Email Template] | Exibição da loja | Determina o modelo de email usado para atualizações de crédito. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Login Options]

![Opções de logon](./assets/customer-configuration-login-options.png)<!-- zoom -->

<!-- [Login Options](https://docs.magento.com/user-guide/customers/login-landing-page.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Redirect Customer to Account Dashboard after Logging in] | Site | Determina o que acontece depois que os clientes fazem logon em suas contas do. Para redirecionar os clientes para o painel da conta, selecione `Yes`. Opções: <br/>**`Yes`**- O painel de conta é exibido quando os clientes fazem logon em suas contas.<br/>**`No`** - Os clientes podem continuar comprando depois de fazer logon em suas contas. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Address Templates]

![Modelos de endereço](./assets/customer-configuration-address-templates.png)<!-- zoom -->

<!-- [Address Templates](https://docs.magento.com/user-guide/customers/address-templates.html) -->

| Modelo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Text] | Exibição da loja | O modelo é usado para todos os endereços impressos. |
| [!UICONTROL Text One Line] | Exibição da loja | Esse modelo define a ordem das entidades de endereço na lista de catálogos de endereços do carrinho de compras do cliente. Progresso durante o check-out. |
| [!UICONTROL HTML] | Exibição da loja | Este modelo define a ordem dos campos de endereço localizados na variável _Endereços de Cliente_ no Painel de administração ([!UICONTROL Customers] > [!UICONTROL Manage Customers]). Esta situação afeta igualmente as pessoas que se encontram _Adicionar novo endereço_ página quando um cliente cria um endereço de faturamento ou de entrega na página da conta. |
| [!UICONTROL PDF] | Exibição da loja | O modelo define a exibição de endereços de faturamento e de entrega nas NFFs, remessas e avisos de crédito impressos. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL Customer Segments]

{{ee-feature}}

![Segmentos do cliente](./assets/customer-configuration-customer-segments.png)<!-- zoom -->

<!-- [Customer Segments](https://docs.magento.com/user-guide/marketing/customer-segments.html) -->

| Modelo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Enable Customer Segment Functionality] | Global | Determina se os segmentos de clientes podem ser usados para criar promoções direcionadas. Opções: `Yes` / `No` |
| [!UICONTROL Real-time Check if Customer is Matched by Segment] | Global | Determina se os segmentos de clientes são validados em tempo real. Opções: <br/>**[!UICONTROL Yes]**- Os segmentos do cliente são validados em tempo real (valor padrão).<br/>**[!UICONTROL No]** - Os segmentos do cliente são validados por uma única consulta SQL de condição combinada. Isso melhora o desempenho da validação de segmentos se houver muitos segmentos de clientes no sistema. No entanto, a validação não funciona com um banco de dados dividido ou quando não há clientes registrados. |

{:style=&quot;table-layout:auto&quot;}

## [!UICONTROL CAPTCHA]

![CAPTCHA](./assets/customer-configuration-captcha.png)<!-- zoom -->

<!-- [CAPTCHA](https://docs.magento.com/user-guide/stores/security-captcha.html) -->

| Campo | [Escopo](../../getting-started/websites-stores-views.md#scope-settings) | Descrição |
|--- |--- |--- |
| [!UICONTROL Enable CAPTCHA on Storefront] | Site | Habilita o CAPTCHA nas lojas associadas ao site do Commerce. Opções: `Yes` / `No` |
| [!UICONTROL Font] | Site | Determina a fonte usada para exibir o CAPTCHA. Para adicionar sua própria fonte, coloque o arquivo de fonte no mesmo diretório da instalação do Commerce e adicione a declaração à `config.xml` arquivo em `app/code/Magento/Captcha/etc`. |
| [!UICONTROL Forms] | Site | Determina os formulários em que CAPTCHA é usado. Opções: <br />`Applying Coupon Code` <br />`Checkout/Placing Order`<br />`Create user` <br />`Login` <br />`Forgot password` <br />`Contact Us` <br />`Change password` <br />`Share Wishlist Form` <br />`Send to Friend Form` <br />`Payflow Pro` (consulte [correção de segurança](https://experienceleague.adobe.com/docs/commerce-knowledge-base/kb/troubleshooting/payments/paypal-payflow-pro-active-carding-activity.html)) <br />`Add Gift Card Code` ![Adobe Commerce](../../assets/adobe-logo.svg)  <br />`Create company` ![Adobe Commerce](../../assets/adobe-logo.svg)  <br /><br />_**Nota:**_ Os formulários Criar usuário, Esqueci a senha e Fluxo de pagamento Pro são sempre ativados quando selecionados. |
| [!UICONTROL Displaying Mode] | Site | Determina quando o CAPTCHA é exibido. Opções: <br/>**`Always`**- CAPTCHA é sempre necessário para fazer logon.<br/>**`After number of attempts to login`** - Essa opção se aplica somente ao formulário de Logon do administrador. Quando selecionado, a variável _[!UICONTROL Number of Unsuccessful Attempts to Login]_é exibido. Insira o número de tentativas de logon que deseja permitir. Um valor de `0` (zero) é semelhante à configuração [!UICONTROL Displaying Mode] para `Always`.<br/>_**Nota:**_Para rastrear o número de tentativas de logon malsucedidas, cada tentativa de logon com um endereço de email e a partir de um endereço IP é contada. O número máximo de tentativas de logon permitidas no mesmo endereço IP é 1.000. Essa limitação se aplica somente quando CAPTCHA está ativado. |
| [!UICONTROL Number of Unsuccessful Attempts to Login] | Site | Especifica o número de vezes que um cliente pode tentar fazer logon antes que a conta seja bloqueada. |
| [!UICONTROL CAPTCHA Timeout (minutes)] | Site | Determina a duração do CAPTCHA atual. Quando o CAPTCHA expira, o usuário deve recarregar a página. |
| [!UICONTROL Number of Symbols] | Site | Determina o número de símbolos que aparecem no CAPTCHA, com um máximo de 8. Você também pode especificar um intervalo, por exemplo, 5-8. |
| [!UICONTROL Symbols Used in CAPTCHA] | Site | Determina as letras (a-z e A-Z) e os números (0-9) que aparecem no CAPTCHA. Símbolos difíceis de distinguir de outros símbolos, como `i`, `l`ou `1`, não estão incluídos no conjunto padrão de símbolos CAPTCHA. |
| [!UICONTROL Case Sensitive] | Site | Determina se os caracteres CAPTCHA fazem distinção entre maiúsculas e minúsculas. Opções: `Yes` / `No` |

{:style=&quot;table-layout:auto&quot;}