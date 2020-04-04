---
layout: post
title:  "Como ficar bêbado eficientemente usando resultados científicos"
category: "blog"
tags: articles portuga
---

# Como ficar bêbado eficientemente usando resultados científicos

Um problema rotineiro e pertinente para muitos jovens é a questão da embriaguez com alcool: como atingir esse estado evitando-se efeitos adversos como vômitos, perca de memória e inconsciência ao mesmo tempo em que se maximiza a extroversão e “alegria” oriundos do consumo em si?

Nessa postagem, irei fazer uma exploração rápida bem como farei sugestões acerca do tema utilizando-se de fontes científicas reputáveis.

Em todo o corpo do texto, irei usar a sigla BAC (Blood Alcohol Content) como significando a concentração de alcool no sangue. Em outras palavras, é a porcentagem em massa do seu sangue como sendo alcool.

## Estimando a concentração do alcool no corpo

A evolução da concentração do alcool no corpo já foi muito explorada pela ciência forense e as estimativas da eliminação do alcool do corpo costumam baseadas na fórmula de Widmark, cuja explanação pode ser melhor ser vista na referência [^1].

Porém para fins de simplicidade, irei considerar que o alcool é imediatamente digerido pelo corpo e irei adotar o modelo adotado por um estudo sueco em universidades [^2], na qual a variante da fórmula de Widmark pode ser expressa como:

![Fórmula da embriaguez]({{ site.url }}/assets/outros/eq_bac.png)

onde 0.806 é a constante de água do corpo, 0.12 é um fator de conversão, BW é uma constante que tem valor 0.58 para homens e 0.49 para mulheres, Wt é a massa em kg do corpo da pessoa, \beta é a taxa de remoção de etanol por hora pelo corpo (que pode ser considerada como 0.017) e t é o tempo desde o consumo.

Porém, nem sempre é possível calcular a concentração de alcool no meio da festa. Sendo assim, uma aproximação útil é considerar que o corpo elimina cerca de ~5g de etanol por hora e que a ingestão é imediata, o que deve significar aproximadamente uma subtração de ~0.015% do BAC por hora.

## Efeitos de curto prazo do alcool

Vou trapaçear nessa seção. Tem um artigo no Wikipedia com uma tabela bem bacana e bonita com isso [^3] na qual só irei dar um copy-paste:

Com essa tabela em mãos, escolha o seu BAC de preferência e proceda para a próxima seção

## Juntando tudo – aplicações práticas em festa

Utilizando das informações nas seções anteriores, uma aplicação prática festiva é delimitar o BAC com os efeitos subjetivos desejáveis, que neste post irei assumir que o desejável é BAC = 0.1% e utilizar-se da fórmula de Widmark para definir a quantidade de alcool a ser ingerida para atingir o BAC bem também estimar uma quantidade de alcool a ser consumida constantemente para manter o BAC aproximadamente constante durante toda a festa.

Usando a massa do meu corpo como exemplo (60kg), basta resolver a eq. de Widmark com t=0 em função da massa de etanol e igual a 0.1 para obter a massa de etanol necessária para entrar no estágio necessário. O resultado é 36g de etanol (30.4g se eu fosse mulher).

Ou colocando em outras palavras, resolva a seguinte equação para x (que é a massa de etanol). Se você tiver massa corporal diferente de 60kg ou for mulher não esqueça de mudar o 60 para sua massa ou o 0.58 para 0.49:

![Fórmula da embriaguez]({{ site.url }}/assets/outros/eq_bac_resolvida.png)

Como a taxa de eliminação de etanol é de $\beta = \frac{0.0017}{h}$, devo calcular também a massa de etanol que devo ingerir a cada hora para manter o BAC,  ou seja, tomar a eq. de Widmark em função da massa de etanol como igual a 0.017. O resultado é ~6.11g de etanol (5.16g se eu fosse mulher).

Existe um nuance ao aplicar na prática as informações aqui: é difícil saber na prática a massa do etanol sendo ingerido, então temos que usar o fato de que densidade do etanol é de 0.789 g / mL. Só que o etanol é diluído em água, o que resultado em uma densidade do líquido como sendo maior. Uma aproximação boa na prática é considerar densidade 0.9 g / mL para destilados de alto teor alcoolico (cachaça e whiskey por ex.) e assumir 1 g / mL para bebidas fermentadas ou de teor alcoolico perto de 10%. Convertendo os resultados acima assumindo que eu só beba destilados, tem-se que eu preciso ingerir cerca de 40mL (34mL se mulher) de etanol no volume da bebida para ficar com BAC=0.1% e 7mL (6mL se mulher) por hora para me manter nesse nível.

Como exemplo concreto, considere uma cachaça de teor alcoolico 40%. Para eu ficar com BAC=0.1%, eu precisaria ingerir 100mL de cachaça (85mL se mulher), e para manter isso durante a festa seria necessário 17mL (15mL se mulher) por hora.

Apesar de eu ter feito as contas para a minha massa e não ter usado modelos mais sofisticados que considerem a altura como os citados na ref. [^1], os números aqui já são uma boa estimativa para você começar a tentar ser um bêbado de precisão.

Porém ainda há uma última pendência:  como medir o volume de bebida consumido na festa? Minha sugestão é você levar uma caneca contigo junto e fazer marcadores nela de 25mL, 50mL e por ai vai. E de quebra você ainda vai ser ecologicamente correto 😉 (em anexo, uma foto de minha caneca mostrando os marcadores, o chá que estou tomando e a cordinha amarrada na própria para nunca a perder)

![Caneca]({{ site.url }}/assets/outros/caneca.jpg)

[^1]: – The Estimation of Blood Alcohol Concentration, Douglas Posey and Ashraf Mozayani. DOI: 10.1385/Forensic Sci. Med. Pathol.:3:1:33

[^2]: – Alcohol use among university students in Sweden measured by an electronic screening instrument, Agneta Andersson, Ann-Britt Wiréhn, Christina Ölvander, Diana Stark Ekman, and Preben Bendtsen

[^3]:  – Wikipedia contributors, ‘Blood alcohol content’, Wikipedia, The Free Encyclopedia, 4 June 2017, 15:01 UTC, <https://en.wikipedia.org/w/index.php?title=Blood_alcohol_content&oldid=783767861> [accessed 5 June 2017 ]
