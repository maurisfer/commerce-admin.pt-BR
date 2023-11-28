---
title: O que é vitrine eletrônica?
description: Saiba mais sobre as páginas e os elementos funcionais que sua loja pode fornecer para respaldar a experiência de compra de seus clientes.
exl-id: 1c64888f-2bc0-4e2e-b7da-0e7182ea67e0
feature: Storefront
source-git-commit: 3ff5807fd0a3ebf2e9d4f9c085852dd7777a1103
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# O que é vitrine eletrônica?

Na implementação do Adobe Commerce ou Magento Open Source, a loja é a parte externa voltada para o público da loja. Ele fornece o conteúdo e os componentes funcionais que seus clientes usam para comprar e comprar.

O caminho que os clientes seguem para uma venda às vezes é chamado de _caminho para compra_ e sua loja inclui os componentes para que os clientes concluam esse caminho. As seções a seguir fornecem uma visão geral dos tipos de página básicos que fornecem valor estratégico: os locais que os clientes geralmente visitam enquanto fazem compras na sua loja. Ao analisá-los, considere os diferentes recursos da loja que podem ser usados em cada estágio da jornada do cliente.

## Home page

Você sabia que a maioria das pessoas gasta apenas alguns segundos em uma página antes de decidir ficar ou ir para outro lugar? Não é longo para causar uma impressão. Estudos mostram que as pessoas também adoram fotografias, especialmente de outras pessoas. Qualquer que seja o design que você escolher, tudo em sua página inicial deve levar os visitantes para a próxima etapa do processo de vendas. A ideia é orientar sua atenção num fluxo coeso de um ponto de interesse para outro.

![Exemplo de página inicial da loja](./assets/storefront-homepage-full.png){width="700"}

## Página do catálogo

As listagens de páginas de catálogo normalmente têm imagens de produtos pequenas e descrições breves e podem ser formatadas como uma lista ou como uma grade. Você pode adicionar blocos, vídeos e descrições ricas em palavras-chave, além de criar designs especiais para uma promoção ou temporada. Você pode criar uma categoria especial para apresentar um estilo de vida ou marca que seja uma coleção de produtos com curadoria de diferentes categorias.

A descrição inicial do produto geralmente fornece aos compradores informações suficientes para merecer uma análise mais detalhada. As pessoas que sabem o que querem podem adicionar o produto aos seus carrinhos e ir embora. Os clientes que compram enquanto estão conectados a suas contas desfrutam de uma experiência de compra personalizada.

![Página de coleção na loja](./assets/storefront-collection-page.png){width="700"}

## Resultados da pesquisa

Você sabia que as pessoas que usam a pesquisa têm quase duas vezes mais chances de realizar uma compra do que as pessoas que dependem apenas da navegação? Você pode considerar esses compradores como _pré-qualificado_.

### [!DNL Live Search]

Com [[!DNL Live Search]](https://experienceleague.adobe.com/docs/commerce-merchant-services/live-search/overview.html) para o Adobe Commerce, sua loja oferece uma experiência de pesquisa rápida, relevante e intuitiva, e está disponível para o Adobe Commerce sem custo adicional.

![Exemplo do Live Search - pesquisar ao digitar](./assets/storefront-search-as-you-type.png){width="700"}

### Pesquisa de catálogo padrão

Com [pesquisa padrão no catálogo](../catalog/search.md), sua loja inclui uma caixa de Pesquisa no canto superior direito e um link para Pesquisa avançada no rodapé. Todos os termos de pesquisa enviados pelos compradores são salvos para que você possa ver exatamente o que eles estão procurando. Você pode oferecer sugestões e inserir sinônimos e erros ortográficos comuns. Em seguida, exiba uma página específica quando um termo de pesquisa for inserido.

![Exemplo de resultados de pesquisa de catálogo padrão](./assets/storefront-search-results-page-full.png){width="700"}

## Página do produto

A página do produto tem muita coisa acontecendo! A primeira coisa que chama a atenção na página do produto é a imagem principal com zoom de alta resolução e galeria de miniaturas. Além do preço e da disponibilidade, há uma seção com guias com mais informações e uma lista de produtos relacionados.

![Exemplo de página de produto da loja](./assets/storefront-product-page-full-m.png){width="700"}

## Carrinho de compras

O carrinho é onde o total do pedido pode ser determinado, juntamente com cupons de desconto e frete estimado e imposto, e um ótimo lugar para exibir seus selos e selos de confiança. É também uma oportunidade ideal para oferecer um último item. Como venda cruzada, você pode selecionar determinados itens a serem oferecidos como uma compra por impulso sempre que um item específico aparecer no carrinho.

![Exemplo de página de carrinho de compras da vitrine](./assets/storefront-cart-full.png){width="700"}

## Página de check-out

O processo de finalização consiste em duas etapas:

1. Informações de envio

   A primeira etapa do processo de finalização da compra é para o cliente completar as informações de endereço de entrega e escolher o método de entrega. Se o cliente tiver uma conta, o endereço de entrega será inserido automaticamente, mas poderá ser alterado se necessário.

   ![Exemplo de página de check-out da loja](./assets/storefront-checkout-shipping-full.png){width="700"}

1. Informações de Revisão e Pagamento

   A segunda etapa do processo de finalização da compra é para o cliente escolher o método de pagamento e, opcionalmente, aplicar um código de desconto.

   >[!NOTE]
   >
   >Embora [!DNL Commerce] permite configurar vários códigos de cupom, um cliente pode aplicar apenas um código de cupom ao carrinho. (Consulte a [Códigos de cupom](../merchandising-promotions/price-rules-cart-coupon.md#coupon-codes) para obter mais informações.)

   ![Exemplo de página de check-out da loja](./assets/storefront-checkout-payment-full.png){width="700"}

A barra de progresso na parte superior da página segue cada etapa do processo de finalização e a _Resumo do pedido_ mostra as informações inseridas até o momento.

>[!NOTE]
>
>A exceção ao check-out em duas etapas se aplica a produtos virtuais e/ou para download. Se houver apenas esses tipos de produtos no carrinho de compras, a finalização será transformada automaticamente em um procedimento de uma etapa, pois as informações de envio não são necessárias.