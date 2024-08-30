---
title: 'O upload de arquivo não está funcionando em admin/portal/#/sites/default/code'
id: 5pFAkaymcuOQMAqUDGPQZK
status: PUBLISHED
createdAt: 2023-09-12T13:37:36.429Z
updatedAt: 2023-09-12T13:37:37.323Z
publishedAt: 2023-09-12T13:37:37.323Z
firstPublishedAt: 2023-09-12T13:37:37.323Z
contentType: knownIssue
productTeam: Portal
author: 2mXZkbi0oi061KicTExNjo
tag: Portal
slug: o-upload-de-arquivo-nao-esta-funcionando-em-adminportalsitesdefaultcode
locale: pt
kiStatus: Backlog
internalReference: 897956
---

## Sumário

>ℹ️ Este problema conhecido foi traduzido automaticamente do inglês.


Ao tentar carregar um novo arquivo em admin/portal/#/sites/default/code, nada acontece. Ao verificar o console no devTools, podemos ver uma mensagem de erro:
"eventTrackerService não está definido"

## Simulação



1. Vá para admin/portal/#/sites/default/code
2. Vá para New -> Upload File -> selecione o arquivo que deseja importar -> clique em create
 ![](https://vtexhelp.zendesk.com/attachments/token/4uSgPeUxG9xAOkTq1HUs8khX6/?name=image.png)
3. Verifique se nada acontece

## Workaround


O WA é criar o arquivo diretamente nesta UI.
Vá para New -> File -> Nomeie seu arquivo e clique em create -> Insira o código e clique em save.




