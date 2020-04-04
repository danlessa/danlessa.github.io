---
layout: post
title:  "Uma breve introdução ao projeto de análise dos ônibus municipais de São Paulo"
date:   2015-11-04
category: "blog"
tags: projects olhovivo geo portuga
---
Irei falar um pouco sobre meu projeto semi-extra-curricular inicialmente:

Eu estava viajando para Cotia algum dia desses, sem saber muito bem o que fazer para o projeto de uma disciplina experimental do curso, e estava zangado com a falta de pontualidade de algumas vans do transporte público. Fiquei imaginando se não haveria uma forma de saber mais sobre o comportamento dos ônibus para que então eu pudesse deter de alguma forma melhor de previsibilidade a respeito destes sem que fosse algo totalmente estocástico.

Bem, a SPTrans, através de sua área de desenvolvedores, disponibiliza uma API e algumas informações sobre seus ônibus, incluindo um serviço para monitoramento em tempo real de sua frota. Foi aí então que surgiu a ideia do projeto.

O projeto essencialmente é coletar dados, muitos dados, das posições de TODOS os ônibus municipais de São Paulo e analisar estes afim de obter curiosidades e testar hipóteses a respeito do comportamento temporal/espacial dos ônibus.

As possibilidades de testes e conclusões que podem vir a ser retiradas são imensas: como os ônibus se comportam nos horários de picos? como é o tempo de viagem? como as velocidades se distribuem? quais vias ficam rápidas ou lentas? a densidade de ônibus atende bem a população atendida? os ônibus saem quando deveriam? chegam quando deveriam? como muda no final de semana? quantos ônibus estão em funcionamento? etc, etc…

Há, talvez, até mesmo uma aplicação pública para este projeto. Talvez um site que informe estatísticas gerais e específicas para regiões ou linhas específicas. Não seria nada mal saber qual é o melhor horário para pegar ônibus caso o critério principal de “melhor” seja ficar menos tempo no ônibus. De forma igual, seria possivelmente bem gratificante ao curioso fuçar e debruçar sobre estatísticas e mapas fartos a respeito dos ônibus. Porém não garanto o site, vai depender das férias. De qualquer modo, todo o resultado e código será disponibilizado publicamente (o que pode ser um convite, caso eu não tenha feito isso até daqui 3 meses)

Atualmente, a coleta é feita através de um Raspberry Pi conectado na internet da USP, o que possibilita uma velocidade muito alta de aquisição (especificamente, uma varredura completa na cidade em menos de um minuto, o que é tão rápido a ponto de ter de fazer a coleta “atrasar” um pouco para dar um pouco de tempo para os ônibus andarem), o que vem gerado cerca de ~3 milhões de dados por dia útil.

Para terminar o post, vou anexar alguns gráficos legais que já sairam de resultado (feitos com aproximadamente uma semana de coleta, ~20 milhões de dados).

![Mapa da velocidade mediana dos ônibus]({{ site.url }}/assets/mapa_velocidade_mediana_onibus.png)

![Tempo de viagem mediano dos ônibus por hora do dia]({{ site.url }}/assets/tempo_mediano_onibus.png)

![Velocidade mediana dos ônibus por hora do dia]({{ site.url }}/assets/velocidade_mediana_onibus.png)
