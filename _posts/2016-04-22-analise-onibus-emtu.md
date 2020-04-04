---
layout: post
title:  "Analise individual dos ônibus da SPTrans e coleta de dados da EMTU"
date:   2016-04-22
category: "blog"
tags: projects olhovivo geo portuga
---
Nos dois meses passados, o projeto dos ônibus tiveram duas atualizações legais:

A primeira é a feitoria do site http://olhovivo.if.usp.br/ onde é possível visualizar alguns dos gráficos e resultados expostos no seminário porém para sua linha de ônibus favorita! O site não está uma coisa exatamente polida, mas já dá para se divertir (e o mais legal da falta de polidez, é observar que somente os dados puros já bastam para fornecer algo bem relevante).

A segunda é que já fiz um hack código para colher dados da EMTU. Chamou-me a atenção a riqueza de detalhes do output resultante (é possível saber inúmeras coisas, como quantidade de assento, tipo de ônibus, empresa operadora, etc etc). Ainda não sei exatamente quais conhecimentos é possível de extrair além do que já foi feito com a SPTrans, porém é algo a ser pensado futuramente.

De brinde, segue um print de posições coletadas por 15min da EMTU. Os scripts em IPython3 para coleta e feitoria desse mapinha estão aqui

![Mapa dos dados]({{ site.url }}/assets/mapa_emtu.png)
