---
layout: post
title:  "O efeito da greve dos caminhoneiros no uso de bicicletas em São Paulo"
category: "blog"
tags: explorations bike portuga
---

Desde segunda passada (21 de maio), está ocorrendo uma paralisação nacional dos caminhoneiros que ganhou o noticiário e os feeds. Congestionamentos e filas quilômetricas foram formadas por veículos automotores sedentos por gasolina assim como coletivos de transporte público passaram a ter circulação restrita.

Intuitivamente, tal cenário iria favorecer um uso maior das bicicletas. Mas qual é o efeito númerico disto?

São Paulo possui um contador de bicicletas na ciclovia Avenida Faria Lima que fornece uma estimativa relativamente acurada do fluxo. O que eu fiz então foi coletar a série histórica dele para obter algum número de antes e depois da greve.

Tem um notebook em Python em https://gitlab.com/danlessa/computacoes/tree/master/Explorations/BikeCET que detalha como foi o processo de aquisição e análise de dados, mas vou cuspir logo o resultado:

![Contagem de bicicletas na Faria Lima]({{ site.url }}/assets/outros/trafego-bicicletas.png)

O domingo da greve foi o domingo mais ocupado do ano por uma margem relativamente folgada, com uns 13% a mais em relação ao segundo colocado. O movimento em média também foi superior ao restante do ano com cerca de 4900 contagens diárias após a greve contra cerca de 3900 antes da greve.

É interessante notar que ao inspecionar o gráfico tomando o domingo como referência, o movimento da sexta-feira sempre decresce ao comparar com a quinta-feira. A exceção foi quando houve o caos na quinta passada – de modo inédito no ano a contagem de bicicletas na sexta foi maior do que na quinta.
