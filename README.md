# Data Visualization: gráficos de composição e relacionamento

Boas-vindas a mais um curso de **visualização de dados** da Alura! 

Esse Github foi produzido com muito carinho para você montar o seu portfólio com as atividades do curso e elaborar suas próprias hipóteses, testar as técnicas exploradas dentro do curso e também adicionar outras durante a leitura das documentações de bibliotecas de visualização de dados com a linguagem Python: **Matplotlib**, **Seaborn** e **Plotly**.

O objetivo deste curso é auxiliar você a utilizar a linguagem Python na análise de dados por meio da agregação de recursos visuais, recorrendo a gráficos como ferramentas de exploração e apresentação dos dados ao seu público. É importante que você tenha um **conhecimento básico** das **bibliotecas de visualização** de Python, bem como das **bibliotecas de manipulação de dados** como **Pandas** e **Numpy**.

## Introdução

Neste curso, vamos construir um portfólio com as análises de duas bases de dados diferentes, explorando cada uma e respondendo aos questionamentos levantados em torno de seus dados. Todas as bases estão no formato CSV e podem ser acessadas por meio do Github.

## Projetos

> Bases de dados:

<ol> 
  <li> Tabela com os PIBs (Produto Interno Bruto) dos estados brasileiros no período de 2002 - 2020</li>
  <li> Tabela com a pontuação do IDEB (Índice de Desenvolvimento da Educação Básica) das escolas à nivel nacional</li>
</ol>

## Paleta de Cores

Como sugestão para escolha da paleta de cores para o seu projeto existem sites como o [Coolor](https://coolors.co/palettes/trending) ou [imagecolorpicker](https://imagecolorpicker.com/).
As cores utilizadas nesse projeto são: 

|Azul||||||
|------|------|------|------|------|------|
| AZUL1 |AZUL2 |AZUL3 |AZUL4 |AZUL5 |AZUL6 |
|#174A7E | #4A81BF | #6495ED| #2596be | #94AFC5 | #CDDBF3 |
|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/AZUL1.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/AZUL2.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/AZUL3.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/AZUL4.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/AZUL5.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/AZUL6.png?raw=true) |

&nbsp;

|Cinza||||||
|------|------|------|------|------|------|
| CINZA1 |CINZA2 |CINZA3 |CINZA4 |CINZA5|BRANCO|
|#231F20 | #414040| #555655 | #A6A6A5| #BFBEBE |#FFFFFF|
| ![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/CINZA1.png?raw=true)  |![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/CINZA2.png?raw=true) |![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/CINZA3.png?raw=true) |![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/CINZA4.png?raw=true) |![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/CINZA5.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/BRANCO.png?raw=true)|

&nbsp;

|Vermelho|||Verde|||
|------|------|------|------|------|------|
| VERMELHO1 |VERMELHO2 |LARANJA1 | VERDE1 |VERDE2 | VERDE3 |
|#C3514E | #E6BAB7 | #F79747|#0C8040 | #9ABB59 |#9ECCB3|
| ![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/VERMELHO1.png?raw=true) |![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/VERMELHO2.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/LARANJA1.png?raw=true)| ![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/VERDE1.png?raw=true) |![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/VERDE2.png?raw=true)|![adicionar desc](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/paleta_cores/VERDE3.png?raw=true)|

&nbsp;

## Visualizações que exploraremos

Na imagem abaixo, apresentamos um diagrama com diversos tipos de **visualização de dados** (criado por [Andrew Abela](https://extremepresentation.com/wp-content/uploads/choosing-a-good-chart-09-1.pdf)) em que é possível perceber **4 subgrupos**, dentre eles:

- Comparação
- Distribuição
- Relacionamento
- Composição

![Diagrama de Visualização de Dados (Andrew Abela - Traduzido por Afonso Rios)](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/imagens/Tipos_Graficos/Diagrama%20de%20Visualiza%C3%A7%C3%A3o%20de%20Dados%20(Andrew%20Abela%20-%20Traduzido%20por%20Afonso%20Rios).png)

Para este curso focamos nos subgrupos da Composição e Relacionamento, levando em conta as observações que gostaríamos de apresentar em nosso portfólio.

### Gráficos de Composição

Neste projeto, vamos explorar diversos gráficos de composição dentre eles:

- Gráficos de Setores (Pizza e Rosca)
- Gráficos de Cascata
- Gráficos de Colunas Agrupadas
- Gráficos de Barras e Colunas Empilhadas
- Gráficos de Áreas
- Gráficos de Inclinação
- Treemap (Gráfico de Árvore)

### Gráficos de Relacionamento

Neste projeto, vamos explorar diversos gráficos de relacionamento dentre eles:

- Gráficos de Dispersão com linha de tendência
- Gráficos de Dispersão com cores
- Gráficos de Bolhas

## Gráficos Produzidos

Para verificar um resumo com os principais gráficos gerados ao longo curso clique nesse [link](https://github.com/alura-cursos/dataviz-graficos-composicao-relacionamento/blob/main/Data_Visualization_gr%C3%A1ficos_de_composi%C3%A7%C3%A3o_e_relacionamento_(gr%C3%A1ficos_produzidos).ipynb)

## Conclusões

Esse curso teve como objetivo apresentar os diferentes tipos de visualização de dados e como escolher qual é o mais adequado para representar as análises de acordo com as perguntas e demandas requisitadas para o problema. Durante o curso, você aprendeu a criar gráficos de composição e relacionamento dos dados partindo do uso das bibliotecas mais utilizadas em Python, personalizar os gráficos e adicionar outros recursos visuais como anotações, destaques, legenda de dados e outras técnicas de visualização. 

Ao final do curso, você será capaz de gerar visualizações personalizadas e voltadas ao tipo de público que você deseja.	

Sinta-se à vontade para fazer o fork desse projeto e construir o seu portfólio 😊
