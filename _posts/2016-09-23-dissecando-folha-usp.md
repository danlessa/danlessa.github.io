---
layout: post
title:  "Dissecando a folha salarial da USP"
date:   2016-09-23
category: "blog"
tags: explorations academia portuga
---
Alguns meses atrás, no período da greve, eu fiz uma dissecação da folha salarial da USP buscando descobrir insights a respeito a crise orçamentária na universidade,  dado que o comprometimento do orçamento com os salários está na ordem de ~95%.

Para tal, eu fiz download da relação completa da folha salarial no Portal Transparência da USP e fiz uma exploração de dados com o stack usual de Python3+Jupyter+Pandas e neste post irei mostrar alguns resultados e fatos obtidos dessa exploração. O código bem como o arquivo salarial utilizado pode ser encontrado em: https://github.com/danilolessa/computacoes/tree/master/analises/transparencia

Observação: os números salariais e associados com estes se referem ao salário bruto, ou em outras palavras é o que a USP efetivamente paga regularmente ao invés de ser o valor que o assalariado recebe realmente. Tal decisão por utilizar o salário bruto se deve por este ser mais “estável” temporalmente dado que indenizações e benefícios não são contabilizados no bruto e também devido ao fato de que essa exploração visa ganhar insight das despesas da universidade em si, sendo então a informação do salário líquido menos relevante nesse âmbito.

Uma segunda observação é que sempre que for utilizado um número anual relacionado com os salários, os benefícios como 13º estarão excluídos por consequência da utilização do salário bruto como critério de cálculo.

## Panorama Geral

Nessa seção, apresento alguns números gerais do salario bem como a distribuição destes. Note que a utilização da mediana se dá devido a interpretação intuitiva desta. A média não é utilizada pois a distribuição salarial não é simétrica e devido a isso ela tende a enviesar os salários para cima quando utilizado como indicador para contextualizar com a situação na USP.

![Distribuição geral dos salários na USP]({{ site.url }}/assets/salarios_usp.png)

Gasto anual aproximado com salários: R$ 3.427.651.958,64 (27.417 pessoas)

Salário mediano na USP: R$ 8.775,31

Proporção de funcionários/docentes ganhando mais que o governador: 8% (2.778 pessoas)

Gasto anual aproximado com salários de funcionários/docentes ganhando mais que o governador: R$ 691.372.729,92

## Funcionários ativos

![Distribuição de salários dos funcionários ativos]({{ site.url }}/assets/salario_usp_ativos.png)

![Salário e tempo de serviço dos funcionários ativos]({{ site.url }}/assets/salario_usp_ativos_2d.png)

Quantidade: 15.370

Salário mediano: R$ 6.898,01

Proporção ganhando mais que o governador: 0.7% (109 pessoas)

Uma exploração especialmente interessante, é analisar o salário mediano de cada função na USP. O resultado entretanto é muito longo para ser embutido nesse post, então peço que visite esse link: http://soc.if.usp.br/~danlessa/misc/folha-usp.html

## Docentes ativos

![Distribuição dos salários dos docentes]({{ site.url }}/assets/salario_usp_docentes.png)

![Salário e tempo de serviço dos docentes]({{ site.url }}/assets/salario_usp_docentes_2d.png)

Quantidade: 6.073

Salário mediano: R$ 13.586,40

Proporção ganhando mais que o governador: 18.4% (1.118 pessoas)

## Docentes aposentados

Quantidade: 2.992

Salário mediano: R$ 16.921,45

Proporção ganhando mais que o governador: 31.3% (937 pessoas)

Bônus: gabinete do Reitor

Adicionalmente, o acesso a folha salarial permitiu visualizar os integrantes do gabinete do Reitor. A relação completa pode ser vista em http://soc.if.usp.br/~danlessa/misc/folha-gabinete-reitor.html

Note a presença de dois cozinheiros, dois auxiliares de cozinha, dois jornalistas, um garçom e quatro motoristas.
