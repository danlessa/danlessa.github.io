---
layout: post
title: "Levantamento de empresas de ônibus rodoviário amigáveis ao ciclista"
date:   2019-04-01
category: "documents"
tags: projects bike portuga
---



Disclaimer: esse documento é colaborativo, propositivo e em caráter eterno de rascunho. Não seja tímido de editar, discutir ou criticar.

## Resumo

Busca-se neste projeto estudar, implementar, divulgar e ramificar um levantamento extensivo e detalhado acerca da permissibilidade do transporte de bicicletas nos ônibus rodoviários no Brasil.

Para tal, serão identificados pontos de importância para os ciclistas brasileiros em diferentes estratos visando a formulação de uma lista de métricas a fim de classificar as empresas operadores de linhas rodoviárias - nas quais adotaremos um método para inferir o posicionamento das mesmas.

Adquirido os dados de um modo suficientemente representativo de todo o universo de linhas rodoviárias, estudará-se então a formulação de uma métrica composta afim de classificar as empresas de acordo com a sua "amigabilidade" ao ciclista. O resultado final será uma planilha extensa e detalhada pública com possíveis usos distintos, no qual cito especificamente a criação de um aplicativo web que simule trechos de ônibus junto a "amigabilidade" ao ciclista.

## Introdução

### Objetivos

**Principais**
* Mapear as necessidades e aflições de um modo representativo ao transportar a bicicleta em ônibus rodoviários.
* Estabelecer métricas que façam correspondência com o objetivo acima.
* Levantar as métricas junto com as empresas operadoras de linhas rodoviárias no Brasil.
* Disponibilizar os resultados obtidos de um modo acessível e fácil de ser consumido.

**Secundários**
* Criar um aplicativo web que possibilite a simulação de rotas de ônibus junto com a exposição das métricas obtidas.
* Explorar ramificações da informação adquirida para no cicloativismo.
* Estudar a possibilidade da criação de um "selo" de empresa amiga do ciclista, para uso das empresas bem colocadas nas métricas.


### Frentes de trabalho

1. Discussão e coleta das necessidades, experiências, expectativas e sonhos dos usuários de bicicleta em relação ao uso de ônibus rodoviário. É importante que saibamos exatamente o que aflige o ciclista na hora de viajar tanto na problemática quanto no perfil, seja ele cicloturista ou competidor, excluido ou elitizado, viajante local ou distante. (2 a 4 pessoas com perfil representativo/experiência diversas? 1-3h de tempo para fazer conversas e discussão)

2. Formulação de um método padrão para coleta de informações. São muitas empresas, então precisamos adotar um método padrão para aferir as características levantadas no ponto 1. E não necessariamente as empresas vão querer se posicionar, então o que fazer nesse caso? Informações levantadas informalmente e/ou pessoalmente são mais úteis que nenhuma informação, mas como que levamos isso em consideração? (2 a 4 pessoas com perfil representativo/experiência diversas? 1-2h de tempo para fazer conversas e discussão)

3. Levantamento das informações. Isso significa contato direto com a empresa. Isso pode ser tanto através do e-mail quanto por telefone ou pergunta direta aos funcionários ou usuários passados. (1 a 4 pessoas com disposição de ceder tempo útil, algo entre 5-20h de tempo para levantar as informações)

4. Visualização das informações. Isso pode ser tanto só divulgar uma planilha quanto para até o desenvolvimento de um aplicativo web que faça a simulação de rotas de ônibus e já dê uma pontuação atrelada a cada linha ou horário. Algo no estilo do buscaonibus.com. Os dados para isso existem e são públicos, mas há a necessidade de um programador. (pessoas que saibam algo de desenvolvimento de aplicativos web)

5. Composição de uma pontuação para cada empresa: como fazemos isso? Damos uma nota de 0 a 100% com qualquer critério? Ou damos selo de amigo do ciclista? É uma discussão interessante de se ter (2 a 4 pessoas com perfil representativo/experiência diversas?, 1-2h de tempo para conversas e discussões)

## Aquisição dos dados

### Metodologia

#### Mapeamento de aflições e constatações

De Vinicius Mundim (UCB):

"Há empresas de ônibus / avião que só aceitam (ou se veem obrigadas a aceitar) bicicletas quando o ciclista apresenta a carteirinha de federado (CBC ou federação estadual), o que acaba por criar uma segregação desnecessária. Mas é um caminho para tentar mapear o cenário.
"

De Leonardo Dal Picolo (UCB):

"
* Ônibus de dois andares (leito e semi leito) tem bagageiros menores e mais gente viajando. É bom checar antes de comprar a passagem, porque no ônibus convencional (apenas um andar) os bagageiros são mais altos e sobra mais espaço. Eu nem tento colocar minha bicicleta em um ônibus de dois andares, principalmente se for rota muito turística e data festiva. Mas se essa fosse a única opção, eu reduziria a bagagem (em volume) ao máximo possível.
* Tirar a roda dianteira e pedais e abaixar/tirar selim geralmente são suficientes quando se coloca a bicicleta dentro de uma caixa ou envolve a bicicleta com papelão. Já levei a bicicleta até sem qualquer proteção, mas isso pode impedir o transporte em alguns casos. A maior preocupação dos motoristas é que a bicicleta não danifique outras bagagens. Se alguém tem receio de desmontar a bicicleta para transportar, acredito que em caso de uma lei específica, provavelmente seria exigido que retirasse ao menos roda dianteira, pedais e selim.
* Nunca me cobraram qualquer valor adicional pelo transporte da bicicleta. Venho transportando bicicleta em ônibus desde 2013, então pode ser que algumas empresas tenham criado regulamento para o transporte de bicicleta nesse tempo. Aparentemente não há lei específica para o transporte de bicicleta.
* Sempre chegar com antecipação, para deixar tudo preparado. Eu converso com as pessoas que vão embarcar no mesmo ônibus (na maior parte das vezes essas pessoas que iniciam a conversa, por curiosidade) e já aconteceu até de me ajudarem/apoiarem na argumentação com motorista mais burocrático.
* Evito o esforço do motorista/pessoa que carrega o bagageiro. Sempre que possível, pergunto onde pode colocar e eu mesmo organizo tudo, no momento que a pessoa reserva para guardar a bicicleta (e toda a tranqueira que acompanha a bicicleta...).

Diante do exposto, ao menos de minha parte, eu não tentaria (muito menos nesse momento político) dialogar para a criação de uma lei específica para o transporte de bicicletas. Digo isso porque aparentemente (pelo menos da minha experiência) ainda é relativamente fácil e grátis transportar a bicicleta no ônibus. No Chile tive que pagar o valor de outra passagem para transportar a bicicleta.
"

### Resultados

#### Resultado conceitual

Uma planilha de prova de conceito está link no https://goo.gl/M18sHJ

São colocadas três métricas: Clareza, Receptividade e Extra. Há também uma métrica composta de Pontuação.

As informações foram coletadas de um modo exploratório através da inspeção direta em websites institucionais, ferramentas de busca online e grupos de discussão online.

A métrica de Receptividade é definida como sendo entre 0 a 4 (inteiros) e se refere ao posicionamento da empresa em relação ao transporte de bicicleta, sempre com base no menor denominador.

| Receptividade | Descrição
| - | -
| 0 | Proibido |
| 1 | Taxado |
| 2 | Obrigatório embalar |
| 3 | Burocrático* |
| 4 | Permitido |
| ? | Desconhecido

\* A empresa coloca empecilhos, como exigir nota fiscal.



A métrica de Clareza é definida como sendo entre 0 a 4 (inteiros) e corresponde ao tanto que a métrica de receptividade é representativa e abraçada pela empresa como um todo. Tal métrica busca tornar possível a mescla entre informações verificadas institucionalmente e informalmente.

| Clareza | Descrição
| - | -
| 0 | Informal: algum motorista deixou
| 1 | Indireto: algum funcionário de médio escalão permitiu
| 2 | Escrito: há um posicionamento via texto não-público, como via chat e e-mail
|3 | Mídia: A empresa se posicionou via redes sociais ou imprensa
|4 | Oficial: A empresa se posicionou publicamente em caráter regulamentado

## Ramificações

### Aplicativo web

Uma forma de expor os resultados obtidos é através de uma aplicativo web que faça a simulação de rotas de ônibus dada a entrada da origem e destino pelo usuário. Para tal, é possível tanto construir uma solução "do zero" utilizando informações contidas na ANTT, ou então é possível fazer parceria com alguns dos sites que já o fazem a simulação, como o buscaonibus.com.br e clickbus.

Uma eventual parceria poderia envolver tanto a cessão da API e dicionário de empresas utilizadas para uma reimplementação em um website próprio, ou poderia ser uma parceria mais integral onde a implementação seria diretamente no website do parceiro.

Caso haja a necessidade de hospedagem, a UCB já se ofereceu de manter o mesmo em seu website.

#### Possíveis parceiros

##### buscaonibus.com.br

A primeira empresa a ser contatada é o buscaonibus.com.br. Obtive uma boa receptividade por parte do CEO e o mesmo está em vias de dialogar com o time da empresa para então dar um feedback.

### Cicloativismo

A realização desse estudo fornece um ingrediente essencial para futuras articulações com a ANTT. Cito aqui o Yuriê da UCB:

"Uma sugestão que tenho é que essa mobilização toda aconteca em conjunto com uma pressão junto à ANTT para que o transporte de bicicleta seja de fato realidade. As normas da ANTT já preveem o transporte de bicicletas em ônibus, mas as empresas descumprem. Tenho alguns contatos lá é posso ajudar nisso.

Inclusive, a ANTT é obrigada por lei a realizar uma pesquisa anual de avaliação dos serviços das concessionárias e empresas. Ao longo dos 15 anos de existência a terceira pesquisa está sendo finalizada. Estou em um grupo junto à CGU que está penando em métodos para baratear a pesquisa e permitir que ela seja realizada anualmente. Já coloquei essa questão do transporte das bicicletas ao grupo, mas posso reforçar.

Como Daniel falou, é importante definir como avaliar o transporte da bicicleta e, pra isso, acho fundamental definir como é o modelo ideal. Podemos conseguir que a ANTT faça uma audiência pública sobre o tema para definir esse padrão."

### Selo de empresa de ônibus amiga do ciclista

### Imprensa

## Conclusões

## Anexo
