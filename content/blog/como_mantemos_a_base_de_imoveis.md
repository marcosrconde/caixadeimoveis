---
title: Como atualizamos e mantemos a base de dados de imóveis
author: Marcos Conde
description: Atualizamos a base de imóveis caixa diariamente para você estar sempre à frente. 
date: 2022-07-28T17:08:33-03:00
draft: false
sidebar: true
sidebarlogo: qachado_logo_transparente
include_footer: true
---

O mercado de imóveis de leilão extrajudicial é bastante dinâmico e boas oportunidades aparecem literalmente todos os dias. Porém, da mesma forma que elas aparecem, podem desaparecer rapidamente. Há imóveis que entram em venda direta online com descontos tão atraentes que desaparecem em menos de 24 ou 48 horas.

Isso foi uma das primeiras coisas que percebi quando comecei a acompanhar as listas de imóveis da Caixa. Para encontrar as melhores oportunidades eu precisaria me manter atualizado e ser rápido.

Porém, quando comecei a procurar os imóveis, me frustei completamente. Seria uma missão quase impossível me manter atualizado procurando apenas no site da Caixa. O sistema de busca e obtenção de informações do site oficial não ajuda e faz com que essa tarefa seja extremamente penosa e demorada.

Logo, idealizei que seria necessário criar um sistema automatizado que literalmente vasculhasse o site da Caixa diariamente e organizasse tudo em um banco de dados contendo todas as informações possíveis sobre os imóveis. Comecei a trabalhar nessa ideia.

Assim começou a história do QAchado. Criamos uma espécie de robô para fazer esse "trabalho pesado". Diariamente o robô QAchado compara as listas de imóveis, identifica as novidades na lista mais atual e também os imóveis que tiveram o preço reduzido, entra na página de cada imóvel no site da Caixa e obtém todas as informações que hoje estão disponíveis na nossa plataforma. As atualizações da nossa base de dados são feitas sempre durante a madrugada. Então aqui vai uma dica valiosa: Todos os dias, por volta das 6:30 da manhã nosso sistema já concluiu as atualizações de todas as modalidades. Fique sempre atento à lista de imóveis "novos", que são aqueles imóveis que apareceram pela primeira vez ou que tiveram algum tipo de alteração de preço ou modalidade.

Ao longo do dia seguinte, a Caixa vai recebendo ofertas pelos imóveis e à medida que isso acontece, os imóveis vão ficando indisponíveis para venda (Venda Direta Online), e os imóveis da Venda Online vão recebendo ofertas e ficando com o status "em disputa". Para conseguir captar esse movimento e não perder, criamos um segundo algoritmo que é executado ao longo do horário comercial. Esse algoritmo "carimba" o imóvel como "em disputa" ou como "indisponível". Essa atualização é feita 5 vezes ao longo do dia.

Assim, conseguimos manter uma base de dados sempre atualizada e, melhor ainda, colocamos tudo isso disponível para que você também possa economizar seu precioso tempo e encontrar excelentes oportunidades de negócio.

Atualmente, nossa base também conta com os imóveis do Santander e da Resale. Nesses casos, a atualização também é diária.

Veja o exemplo abaixo:

![oferta com desconto de 90% em SP](/blog/images/imovel_desconto_SP_QAchado.png)

Esse imóvel em bairro nobre de São Paulo entrou em venda direta com 90% de desconto, de R$712 mil (valor de avaliação) por apenas R$71.200 de lance inicial. E para melhorar ainda mais, o imóvel está desocupado e aceita financiamento habitacional. Óbvio que atraiu a atenção e houve disputa. Ainda assim, o desconto final para o comprador que fez a melhor oferta foi de mais de 60%.  

É ou não é incrível? 

Experimente usar nossa plataforma para navegar pelos milhares de imóveis com desconto da nossa base de dados?

<a href="https://app.qachadoimoveis.com" target="_Blank">**Cadastre-se grátis e acesse aqui**</a>




