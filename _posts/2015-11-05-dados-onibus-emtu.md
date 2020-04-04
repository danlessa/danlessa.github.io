---
layout: post
title:  "Dados dos ônibus da EMTU"
date:   2015-11-05
category: blog
tags: projects olhovivo geo portuga

---
Ao contrário da SPTrans, a EMTU não disponibiliza uma área de desenvolvedores nem nenhuma API. Porém eles possuem rastreamento em tempo real no site e em app para smartphones, o que é sinal de que talvez há algum jeito.

Investiguei o site de rastreamento online, e descobri algumas coisas:

* O serviço de rastreamento é fornecido por uma empresa terceirizada (http://www.noxxonsat.com.br/)
* Este serviço aparenta utiliza JSON para fornecer dados das rotas e posições dos ônibus, de forma análoga com o Olho Vivo

Fuçando repetidamente alguma linha de ônibus, cheguei a conclusão que os dados podem ser obtidos por JSON através do link http://bustime.noxxonsat.com.br/bustime?linha=LINHA&_=????, onde LINHA é simplesmente o código de linha da EMTU e o ??? é um número estranho que ainda não descobri o que é.

Ainda não olhei muito a estrutura resultante, mas ela parece abranger posições dos ônibus, informações (incluindo traçados e pontos) das linha em específico e também horário de partida.

Possívelmente irei pensar numa forma de coletar dados da EMTU nas férias
