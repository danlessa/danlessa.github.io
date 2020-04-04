---
layout: post
title:  "Fazendo mapas interativos de relevo e inclinação usando a API do Google Maps e/ou dados públicos"
date:   2018-04-14
category: "blog"
tags: projects geo portuga
---

Oi pessoal! Alguns dias atrás eu estava passando o tempo e depressão caçando alguns morros épicos para subir de bicicleta (me julguem) e começei a pensar:

“Bem que poderia exisitir um jeito fácil de visualizar os morros aqui né?”

[SPOILER: http://fap.if.usp.br/~danlessa/apps/elevation-map/elevation.html]

E bem, há muito tempo busco algum mapa de relevo que fosse realmente prático e informativo no sentido de eu olhar nele e pensar “aqui estão as ruas e aqui estão os morros”. Até existem os mapas de contorno, mas a verdade crua é que é horrível enxergar aquelas linhas de contornos quando você está olhando o mapa das ruas também. Sem falar que existem poucas fontes de mapas de contorno com uma precisão adequada para uso urbano.

Resolvi resolver com o meu próprio teclado. Usando a API do Google Maps, existe uma forma fácil de obter a altitude associada a uma coordenada qualquer (https://developers.google.com/maps/documentation/elevation/start). Fiz então um grid de diversos pontos em SP para obter a elevação e depois passei um interpolador cúbico para ter uma aproximação contínua do mapa de relevo. O resultado é a figura 1, no qual usei a biblioteca tilemapbase para gerar mapas com o OpenStreetMap. O código-fonte tá aqui ó: https://gitlab.com/danlessa/computacoes/tree/master/Explorations/Altitude%20map.

![Inclinação perto da USP]({{ site.url }}/assets/mapa-interativos/inclinacao-usp.png)

![Elevação perto da USP]({{ site.url }}/assets/mapa-interativos/altitude-usp.png)

O legal de usar o Elevation API é que você pode obter dados de qualquer parte do globo. Como brincadeira, fiz os mesmos mapas para Maringá/Marialva lá no Paraná e também para a minha cidade natal de Ariquemes/RO nas figs. 3 até 6:

![Inclinação em Maringá]({{ site.url }}/assets/mapa-interativos/inclinacao-maringa.png)

![Elevação em Maringá]({{ site.url }}/assets/mapa-interativos/altitude-maringa.png)

![Inclinação em Ariquemes]({{ site.url }}/assets/mapa-interativos/inclinacao-ariquemes.png)

![Elevação em Ariquemes]({{ site.url }}/assets/mapa-interativos/elevacao-ariquemes.png)

Porém, por mais fácil que seja usar a API do Google, ele possui precisão limitada (cerca de 125m em São Paulo). Felizmente, existem dados topológicos abertos disponíveis pela prefeitura de São Paulo, os quais possuem uma precisão e amostragem muito maior (http://geosampa.prefeitura.sp.gov.br/PaginasPublicas/_SBC.aspx#). Como eu fiz as coisas estão no link do repositório que citei acima. O resultado são as figs 7 e 8, que possuem uma resolução excepcional perto do que encontrei por ai.

![Inclinação perto da USP]({{ site.url }}/assets/mapa-interativos/inclinacao-sp.png)

![Elevação perto da USP]({{ site.url }}/assets/mapa-interativos/altitude-sp.png)

Só há então um entrave final: hoje em dia ninguém usa uma imagem impressa para se guiar. Para facilitar a vida de todos, fiz um overlay usando API de Javascript do Googlemaps para sobrepor as imagens geradas em um mapa interativo. Resultado final: http://fap.if.usp.br/~danlessa/apps/elevation-map/elevation.html. Se quiser ver como foi feito, é só ver a fonte da página – 100% client-side.

Fiquei feliz com as coisas.
