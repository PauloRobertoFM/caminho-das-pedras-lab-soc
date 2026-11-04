# Tickets duplicados

## O que aconteceu
A automação abria vários chamados para a mesma vulnerabilidade no mesmo ativo.

## Causa raiz
A busca por chamados existentes olhava só uma janela fixa de tickets recentes. Os antigos saíam da janela e a automação deixava de enxergá-los.

## Lição
Busque por estado (abertos), não por idade ou posição.

## O que fazer diferente
- Garanta que repetir a execução não crie duplicatas.
- Teste a automação com muitos chamados antigos.

> Status: rascunho. Será expandido com a versão didática e ilustrada.
