---
title: 'A interface do usuário do checkout envia o hífen no código postal para o orderForm'
id: 3cqrBqq5x8nixjAFt8BxCx
status: PUBLISHED
createdAt: 2024-01-16T12:37:56.497Z
updatedAt: 2024-01-16T12:37:57.041Z
publishedAt: 2024-01-16T12:37:57.041Z
firstPublishedAt: 2024-01-16T12:37:57.041Z
contentType: knownIssue
productTeam: Checkout
author: 2mXZkbi0oi061KicTExNjo
tag: Checkout
slug: a-interface-do-usuario-do-checkout-envia-o-hifen-no-codigo-postal-para-o-orderform
locale: pt
kiStatus: Backlog
internalReference: 937692
---

## Sumário

>ℹ️ Este problema conhecido foi traduzido automaticamente do inglês.


A interface do usuário do checkout envia um hífen para o código postal para o formulário de pedido, causando problemas no cálculo de SLAs quando um país tem 7 dígitos + o hífen. Isso acontece porque o módulo Logistics considera o hífen como um dígito e depende de como as taxas de envio foram registradas na política de envio.

Portugal e Japão são os únicos nesse cenário.

## Simulação



- Tenha uma conta em Portugal ou no Japão;
- Após adicionar produtos ao carrinho, digite o código postal;
- O produto pode ser mostrado como indisponível

## Workaround



- Revise as taxas de envio para incluir uma faixa mais ampla.


