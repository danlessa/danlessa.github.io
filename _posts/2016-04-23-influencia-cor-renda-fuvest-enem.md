---
layout: post
title:  "Influência da cor autodeclarada e da renda familiar no ingresso pela Fuvest e nas notas do ENEM 2014"
date:   2016-04-23
category: "blog"
tags: explorations vestibular portuga

---
Desde semana passada, ao ouvir algum debate a respeito de cotas no ingresso em universidades públicas, uma certa questão me ataca: as cotas raciais/sociais realmente se justificam ao analisar e comparar dados socioeconômicos dos vestibulando?

## Influência da renda – Fuvest

No que tange as cotas sociais, o efeito da renda é indiscutível. Basta uma verificada rapida no site da Fuvest para visualizar como que a distribuição de matriculados apresenta um perfil mais elitizado do que a distribuição de ingressantes. (clique aqui para ver estat. de inscritos) (clique aqui para ver estat. de matriculados). Por incrível que pareça, não é possível notar uma vantagem para alunos de colégio particular ao checar a proporção de inscritos x matriculados, porém suponho duas coisas: poucos alunos de colégio público sequer tentam a Fuvest e também acredito que o PASUSP tenha alguma influência nessa equidade. (Ao avaliar as estatísticas oriundas de 2001, nota-se que a proporção de matriculados oriundos de colégios particulares aumenta em relação aos inscritos, o que talvez ateste a hípotese do PASUSP como agente de equidade)

EDIT: Ao consultar o último censo escolar, nota-se que ~19% dos estudantes paulistas são oriundos de colégios particulares. Apesar disso, ~60% dos inscritos na Fuvest vem de particulares. É algo a se refletir.

![Inscritos na Fuvest 2015]({{ site.url }}/assets/fuvest1.png)

![Matriculados na Fuvest 2015]({{ site.url }}/assets/fuvest2.png)

![Inscritos na Fuvest 2001]({{ site.url }}/assets/fuvest3.png)

![Matriculados na Fuvest 2015]({{ site.url }}/assets/fuvest4.png)

Porém há a observação de que cursos de alta concorrência no vestibular apresentam perfil de matriculados bem mais elitizado na renda e também maior proporção de alunos oriundos de colégios particulares em relação ao perfil de inscritos.

Em específico, ao analisar as estatísticas para o ingresso em medicina no FMUSP em 2015, nota-se por exemplo que a proporção de candidatos inscritos no vestibular com renda familiar abaixo de 2SM e acima de 20SM são de 9% e 12.6%. Ao olhar a proporção de matrículados, a proporção respectiva é de 3.7% e 31.3%. Aparentemente, possuir a renda familiar alta pode aumentar a chance de passar no vestibular em ~9x em relação a possuir uma renda familiar baixa (e essas estatísticas não são isoladas, nos anos anteriores são ainda mais discrepantes). É possível notar também que a proporção de oriundos de colégios particulares sobem de 66% para 77% na relação ingressantes x matrículados.

*Inscritos para o FMUSP em 2015*
![Distribuição de renda dos inscritos na FMUSP em 2015]({{ site.url }}/assets/fuvest5.png)

*Matriculados no FMUSP em 2015*
![Distribuição de renda dos matrículados na FMUSP em 2015]({{ site.url }}/assets/fuvest6.png)

## Influência da cor declarada – ENEM 2014

Normalmente, o argumento principal contra medidas que visem a inclusão racial na universidade se passa pela ideia de que “Não existe discrepância racial, mas sim uma social. Como as minorias e os oprimidos normalmente pertencem a classes sociais menos privilégiadas, então a utilização de medidas que mirem exclusivamente a renda ou oriundos de escolas públicas bastam”. Basicamente é a ideia de que problemas raciais são na verdade sintomas de problemas sociais.

Uma forma simples de verificar ou não tal argumento em um ponto de vista quantitativo seria através da comparação do ingresso universitário entre vestibulandos de diferentes cores declaradas mas mesma faixa de renda familiar. A utilização somente de estatísticas raciais não é correta pois é bem conhecido de que a população PPI possui menor renda no Brasil do que os brancos, e como visto na seção anterior, a renda influi nos índices de matrícula.

Infelizmente a Fuvest fornece somente dados consolidados na forma de proporção de candidatos que possuem determinada cor declarada, sendo assim impossível cruzar com a faixa de renda familiar. Porém, o INEP divulga anualmente microdados do ENEM (link), os quais podem ser usados para o cruzamento e portanto fazer a comparação descrita no paragrafo anterior, porém utilizando-se das notas do exame ao invés de índices de matrícula.

Fiz um script em Python3 (link) que carrega esses microdados, converte em um formato binário para maior eficiência (afinal são ~10 milhões de inscritos) e disso um gráfico que cruze a renda bem como a cor declarada. O resultado das medianas da pontuação total no ENEM 2014 para candidatos no estado de São Paulo é esse:

![Distribuição da mediana das notas gerais do ENEM 2014 por renda e cor - São Paulo]({{ site.url }}/assets/enem2014_sp.png)

Essencialmente, o fato de alguém ser branco dá em mediana quase 200 pontos de vantagem sobre um preto no ENEM (a discrepância é ainda maior se esse alguém for amarelo). O mais surpreendente é que essa discrepância não desaparece conforme a renda aumenta, mas sim se acentua. Na verdade, a discrepância entre todas as cores se acentuam. O que será que causa isso?

Adicionalmente, fiz também os mesmos gráficos para o Brasil todo, Rondônia, Pernambuco e Minas Gerais:

![Distribuição da mediana das notas gerais do ENEM 2014 por renda e cor - Brasil]({{ site.url }}/assets/enem2014_br.png)

![Distribuição da mediana das notas gerais do ENEM 2014 por renda e cor - Rondônia]({{ site.url }}/assets/enem2014_ro.png)

![Distribuição da mediana das notas gerais do ENEM 2014 por renda e cor - Pernambuco]({{ site.url }}/assets/enem2014_pe.png)

![Distribuição da mediana das notas gerais do ENEM 2014 por renda e cor - Minas Gerais]({{ site.url }}/assets/enem2014_mg.png)




Ao observar Minas Gerais e o Brasil todo, nota-se que os índios estão numa situação ainda pior que os pretos e pardos no que tange a pontuação total no ENEM. (Eu não grafiquei amarelos e indios nos outros devido a pequena população nos outros estados. Recomendo também cautela ao avaliar os amarelos, dado que tal cor é associada no Brasil a várias culturas diferentes, tanto latinas quanto orientais, enquanto que em SP é quase que exclusivamente aos orientais)

A hípotese de discrepância racial como sendo sintoma de discrepância social obviamente não se concretiza. A renda não parece ser o único responsável isolado por termos menos pessoas PPI nas universidades do que o esperado. Pelo contrário, a renda acentua as diferenças raciais.

Eu sinceramente não sei muito como explicar esse resultado estranho. Minha hípotese pessoal é de que talvez cada cor tenha maior associação com culturas específicas que influenciam na hora do vestibular. Talvez os amarelos possuam uma nota maior pois há uma cultura associada de pressão dura sobre os jovens no que tange aprovações. Talvez haja uma estigmatização dos PPI que influencie diretamente na hora do vestibular, ou talvez a cultura dos PPI simplesmente não esteja de acordo com o avaliado no ENEM. De qualquer modo, me abstenho de tentar fornecer uma conclusão definitiva.
