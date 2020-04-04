---
layout: post
title:  "Evolução histórica do questionário sócioeconômico da Fuvest"
date:   2017-10-25
category: "blog"
tags: explorations vestibular portuga
---

## Resumo
Realizei uma coleta de dados históricos do questionário socioeconômico da Fuvest desde 2001 e com isso foi feito uma exploração a fim de prover insight sobre questões básicas como: onde andam os negros da USP? E o pessoal do colégio público? E as mulheres e os pobres? Ao postular idealismos como a população dos inscritos na FUVEST ser idêntico com a população geral bem como escolha da carreira não sofrer influência da condição humana do candidato, conclui-se unicamente com base nos fatos númericos do questionário de que há uma anomalia negativa significante em relação ao ingresso da população PPI que não será resolvida da maneira que está até o século seguinte. Do mesmo modo, há uma discrepância crescente em tendência entre homens e mulheres concomitante com a desigualidade econômica na USP sutilmente crescer. Mas nem tudo é ruim: até 2020 os estudantes de escolas públicas estarão em nível de igualidade com os das particulares no que tange a probabilidade frequentista de ser aprovado no vestibular.

## Introdução
Apesar da FUVEST não divulgar de forma acessível e fácil seus dados para análise temporal de forma abrangente, é possível através da utilizando de técnicas de data mining coletar seus dados dos questionários socioeconômicos para descobrir tendências ao passar dos anos (o código está aqui: https://github.com/danilolessa/computacoes/tree/master/analises/fuvest, cuidado com as gambiarras)

As informações aqui contidas são resultados bastante preliminares e limitadas a informações globais de toda USP. Pede-se cautela ao extrapolar as conclusões aqui enunciadas pois alguns dos resultados são sutis e exigem entendimento dos pressupostos por trás deles. Em específico a FUVEST possui notas de corte diferenciadas por carreiras, o que pode trazer a tona artifícios como o paradoxo de Simpson, o qual requer exploração de forma mais específica afim de investigar a verdade.

É importante ter em mente de que os resultados aqui foram baseados na comparação entre os inscritos vs matriculados e isso torna a análise incompleta por não considerar a população que deixa de se inscrever na FUVEST.

Em específico, a análise utilizou-se dos seguintes postulados para retirar conclusões:

A população de inscritos na FUVEST representa bem a população geral
As opções de cursos são aleatórias, isto é: a condição de alguém não a torna propícia estatisticamente a escolher determinada carreira
Para cada seção, foi feito um gráfico e regressão de evolução histórica ano a ano a respeito do tema junto com alguns comentários gerais.

## Cor

![Evolução da cor entre os matrículados]({{ site.url }}/assets/evolucao-questionario-fuvest/cor.png)

Nesse gráfico e regressão é possível reconhecer alguns fatos:

* Há nitidamente uma anomalia positiva em relação aos amarelos (asiáticos) e anomalias negativas em relação aos PPI no que tange a fração geral de matrículados vs inscritos.
* Os pretos vem crescendo em sua fração numa taxa média de 0.26% ao ano enquanto os pardos vem crescendo em relação a 0.22% ao ano. Ao comparar com a taxa geral e para os brancos de 0.15% além da taxa de 0.11% para os amarelos, parece existir uma tendência para a diminuição da discrepâncias nas anomalias na fração exceto para os indígenas
* Os indígenas apresentam uma taxa de 0.13% ao ano, o que significa que em média eles estão perdendo participação em relação a taxa geral. Sinal de políticas ineficientes?

No ritmo linear atual, levaria o seguinte tempo para que cada cor tivesse a mesma proporção de participação na fração geral:

| Cor  | Brancos  | Amarelos  |  Pretos  | Pardos  | Indígenas |
|---|---|---|---|---| --- |
| **Ano**  |  2087 | - | 2100  | 2047  | -  |

## Renda familiar mensal

![Evolução da cor entre os matrículados]({{ site.url }}/assets/evolucao-questionario-fuvest/renda-familiar.png)

Nota-se que o grupo com maior crescimento linear na fração matrículados/inscritos é o de renda média inferior a 1SM. Adicionalmente, inscritos com renda média abaixo de 2SM e rendimento acima de 15SM apresentaram crescimento na fração. Em outras palavras, há uma tendência de um aumento nos extremos.

![Evolução da cor entre os matrículados]({{ site.url }}/assets/evolucao-questionario-fuvest/renda-inscritos-matriculados.png)

Ao interpolar a renda familiar mensal média dos matrículados e inscritos, há um outro resultado interessante: o coeficiente angular dos matriculados é ligeiramente maior do que o dos inscritos, o que indica que em média, os inscritos na FUVEST estão com o passar do tempo com menor renda em relação aos matriculados.

Em suma, parece existir uma tendência do aumento de desigualdade econômica entre os alunos da USP.

## Gênero

![Evolução da cor entre os matrículados]({{ site.url }}/assets/evolucao-questionario-fuvest/fracao-genero.png)

Os homens apresentam maior probabilidade em média de serem aprovados na USP do que as mulheres, e essa discrepância está aumentando a cada ano com uma boa concordância com a regressão linear.

## Escolas

![Evolução da cor entre os matrículados]({{ site.url }}/assets/evolucao-questionario-fuvest/fracao-escola.png)

Ao analisar o coeficiente angular, o único que ficou acima do coeficiente geral foram a dos candidatos provindos somente de escola pública. Nota-se a fração de inscritos vs matrículados dos alunos oriundos de colégios particulares permaneceu relativamente constante enquanto que nos últimos anos os colégios públicos se aproximaram bastante destes em fração (especialmente entre 2006 e 2010).

Se mantida a tendência linear, levará-se o seguinte tempo para ter equalidade no que tange a fração de inscritos/matrículados em relação ao conjunto total:

## conclusões

Relembrando os postulados do começo:

* A população de inscritos na FUVEST representa bem a população geral
* As opções de cursos são aleatórias, isto é: a condição de alguém não a torna propícia estatisticamente a escolher determinada carreira

Se esses postulados forem verdade (o que não são), tem-se as seguintes conclusões:

* As políticas para os PPI no que tange ingresso a universidade são insuficientes a médio prazo, e no caso dos indígenas não são suficientes nem a longo prazo (a diminuição deles só diminuirá na tendência atual)

* A distribuição de renda no vestibular não parece estar sendo corrigida em tendência e de fato parece que está ocorrendo um acirramento sútil da mesma

* Há uma discrepância crescente entre homens e mulheres

* As políticas afirmativas para alunos somente de escolas públicas parece estar sendo eficaz, porém o mesmo não ocorre para os que são somente parcialmente.

Apesar dessas conclusões, há de se considerar que elas são válidas perante os postulados afirmados e eles não são verdadeiros. A população de inscritos não representa a população geral e tentar acontar por isso é algo não trivial, do mesmo modo que há carreiras que estatisticamente tem maior propensão a atrair pessoas de determinados grupos, o que pode ocasionar o efeito conhecido como Paradoxo de Simpson (https://en.wikipedia.org/wiki/Simpson%27s_paradox) na qual o resultado consolidado pode estar bastante distante da realidade devido a cursos concorridos atrairem especialmente pessoas de determinados grupos, o que ocasiona uma inflação no número de inscritos deste grupo.
