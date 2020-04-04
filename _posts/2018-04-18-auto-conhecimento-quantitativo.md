---
layout: post
title:  "Auto-conhecimento quantitativo – introspecção na era do Big Data"
category: "blog"
tags: explorations personal portuga
---

A partir das próximas semanas vou começar a fazer alguns posts de um tema que de certo modo me fascina: o uso da análise de bases de dados pessoais extensas como forma de gerar auto-conhecimento. Especificamente, utilizando eu como cobaia.

Para fazer isso, eu farei o uso de três base de dados dos quais eu preenchi diariamente por boa parte do ano passado assim como por todo esse ano:

* Humor e atividades feitas durante o dia, através do Daylio.
* Quantidade e qualidade do sono, através do Sleep as Android.
* Atividades físicas e informações gerais de saúde através do Google Fit.

![Google Fit]({{ site.url }}/assets/auto-conhecimento-quantitativo/google-fit.png)

![Daylio]({{ site.url }}/assets/auto-conhecimento-quantitativo/daylio.png)

![Sleep as Android]({{ site.url }}/assets/auto-conhecimento-quantitativo/sleep.png)

Os três programas possibilitam a exportação de todos os dados gerados via .csv, e com isso eu aplicar todo meu arcabouço de ferramentas de análise sobre eles.

Como uma brincadeira inicial, eu decidi explorar um pouco o meu humor usando os dados do Daylio, que é um diário virtual no qual permite você adicionar pontos no tempo representando seu humor numa escala de 5 pontos (péssimo / ruim / médio / bom / excelente) junto com as atividades que você fez durante o dia, os quais são configuráveis pelo usuário.

Uma primeira exploração consiste em tirar médias semanais da escala de humor, que pode variar entre 0% e 100%:

![Média semanal do meu humor nos últimos 6 meses]({{ site.url }}/assets/auto-conhecimento-quantitativo/humor-medio.png)

Nitidamente, as férias do final do ano deram um impulso de imédiato no humor, para depois decair para a média de sempre. Um fato curioso é que o maior poço da série histórica está localizada bem na semana anterior de volta as aulas.

Porém a maior oportunidade para gerar auto-conhecimento reside em associar as atividades ou eventos do dia com o humor. Fazendo isso temos a figura seguinte, o qual é uma tabela contendo o que aconteceu, a contagem do tanto que aconteceu e a pontuação de humor:

![Humor de acordo com a atividade feita (em %)]({{ site.url }}/assets/auto-conhecimento-quantitativo/humor-atividades.png)

A média do humor geral, para fins de comparação, é de 61.9%. Um cuidado que deve existir ao interpretar a tabela é o caráter subjetivo e pessoal dela assim como o fato dos dados não serem homogêneos – as vezes eu altero as configurações e com isso algumas atividades deixam de ser marcados ou então passam a ser marcadas.

As atividades com uma interpretação pessoal minha mais distinta são:

* Passeio – significa vagamente que eu não frequentei os ambientes de costume ou rotineiros. Pode significar tanto um passeio convencional quanto o mero ato de ir para um lugar diferente fazer algo que não necessariamente é lazer.
* Social – é o ato ambíguo de socializar. Pode ou não pode ser lazer – apenas significa que eu me senti socializado.
* Cycling – coloco somente quando faço uma pedalada “épica”, normalmente acima de 20km. Associado a passeios ou trajetos longos.
* Date – significa que eu dediquei um tempo individualizado para alguém.
* Service – destinei tempo a fazer coisas de rotina pessoal – limpar quarto, consertar bicicleta, etc
* Formal – atividades onde eu precisei ficar sério, como reuniões por exemplo

Dito isso, acho que as conclusões que consigo tirar da tabela ao considerar as peculiaridades do que vem a significar cada atividade vem a ser:

* Procastinar não é legal. Não faz bem para a felicidade e nem para fazer coisas.
* Ao invés de procastinar, talvez seja melhor tirar um tempo para passear ou tentar fazer a rotina em um ambiente diferente. * A métrica “passeio” é o fator mais significativo para o bem-estar. Mudar o ambiente faz bem para a mente.
* Socializar é importante também. Junto com passear, é o atríbuto mais associado ao bem-estar. Pena que sou tímido, mas não é por falta de vontade.

Para mim foi surpreendente que a variável “passeio” se destacou tão bem ao fazer essa comparação direta. Eu adotei um critério um tanto liberal para caracterizar o meu dia como tendo “passeio” e isso me fornece um aprendizado curioso: existe uma certa efetividade em se rotacionar o ambiente onde frequenta.

De qualquer modo, isso tudo é o começo. A maior potencialidade das bases de dados é quando se há o cruzamento entre elas e começa-se a considerar a co-dependência entre todos os fatores. Nessa análise simplista, eu apenas calculei uma média sem muitas hípoteses. Ainda assim, achei promissor.

Até a próxima!
