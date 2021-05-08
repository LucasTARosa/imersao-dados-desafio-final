# Olá a todos! 😃

# Projeto de data science aplicado em "drug discovery" 📊


Este projeto, que também é o meu primeiro projeto de data science, é o projeto de finalização da imersão de dados fornecida pela Alura. 
A imersão de dados da Alura foi um evento que ocorreu durante uma semana, ensinando conceitos de data sciece. Durante a sua duração aprendemos como trabalhar com python para a criação de tabelas, diferentes tipos de gráficos, correlações e chegando a utilizar diferentes modelos de "machine learning" para tratamento dos dados. Este foi o meu primeiro contato com a linguagem python (e possuo baixa experiência em qualquer outra linguagem) e com machine learning, portanto, todos os conteúdos abordados em aula foram novidade. Novidades estas que aprendia feliz, mesmo que as vezes a ficha demorasse um pouco para cair.

## O projeto 📈
### Justificativa e bibliografia
### Resumo expandido
Para o projeto final, foi realizado o tratamento dos mesmos dados utilizados em aula, mas desta vez com toda a liberdade para tratar os dados como eu quis. Os dados estavam separados em duas tabelas diferentes, chamadas de dados experimentais e resultados. A tabela de dados experimentais possuia informações acerca de diferentes experimentos e suas respectivas condições, como tempo, dosagem, droga utilizada e o controle. Estas informações eram acrescidas de como eram alterados 712 genes diferentes e como a variação nos genes afetavam o número (a população) de 100 células diferentes. Já a tabela resultado nos forneceria uma correlação com a tabela dado (através do id de cada experimento), onde eram associdados diferentes mecanismos que poderiam ou não estar ocorrendo naquele determinado experimento, ou seja, quais vias metabólicas poderiam estar sendo ativadas. 

O objetivo deste trabalho foi encontrar correlações entre diferentes genes e se e como os mesmos afetavam a população de determinada célula. Outro objetivo deste trabalho foi a busca por um modelo de machine learning que conseguia modelar satisfatoriamente se um determinado composto, dado as condições experimentais, expressões gênicas e a população de células iria ter atividade ou não, independente da via metabólica ou da quantidade de vias ativadas. Para alcançar estes objetivos, o trabalho foi separado em três grandes etapas, sendo subdividas em outras etapas menores.
#### Etapa 1
Nesta primeira etapa foi realizada a importação de diferentes ferramentas que serão utilizadas ao longo do projeto, assim como a importação dos dados experimentais e de resultados. Foi realizado um primeiro contato e entendimento dos dados experimentais, entendendo as frequências, proporções e quantidade de categorias que os experimentos foram conduzidos. Desta forma, foi constatado que as 10 drogas com maior número de experimentos representavam 0,3% do volume de drogas, mas 16% do volume de experimentos. Desta forma, para focar no estudo sobre o efeito destas 10 drogas, o volume de dados foi limitado para os experimentos que foram realizados com elas.
#### Etapa 2
Após a análise inicial, foi feito o correlacionamento entre os primeiros 75 genes com as primeiras 75 células, de forma a entender se possuiam uma resposta proporcional, neutra ou inversamente proporcional, ou seja, se a medida que uma expressão gênica aumentava a população das células aumentavam, diminuia ou se mantinha. Estes números de genes e de células foram escolhidos para limitar o volume de informação a ser tratada, devido ao tempo para a realização do projeto. Foram escolhidas três genes diferentes e como eles influenciavam na população de uma célula. Foram estudados detalhadamente cada um dos genes e quais drogas afetavam sua expressão genômica, além de correlações mais diretas com a população da célula em função do aumento ou diminuição destas expressões genômicas.
#### Etapa 3
Nesta etapa foi realizado o tratamento dos dados da tabela resultados de acordo com o objetivo de estudo da machine learning. Desta forma, foi contruída uma nova coluna ao final que retornava um valor booleano (verdadeiro ou falso) para a seguinte pergunta "Este experimento ativou ao menos uma via metabólica?". Após esta etapa, a tabela que continha os dados experimentais foi trabalhada de forma a acrescentar esta informação de ativação ou não de ao menos uma via metabólica para aquele experimento, chamada de moa. O trabalho continuou com a transformação dos dados de "tratamento", "tempo" e "dose" como valores binários, sendo criadas novas colunas que apresentavam o valor 1 para quando ocorria aquela condição experimental ou 0 para quando não ocorria. Esta etapa é importante para a utilização em machine learning, pois alguns modelos só podem levar em consideração números, portanto, para que as condições experimentais tivessem um peso na modelagem, foi necessária esta transformação. Por fim, os dados foram aplicados em diferentes modelos de machine learning até que se obtivesse um modelo com resultado satisfatório. 
### Conclusão
Foi possível encontrar correlações significativas entre três diferentes genes, descobrindo qual a droga que mais afetava a expressão gênica e como a alteração gênica alterava a população de uma determinada célula, respectivamente para cada um dos genes estudados. Assim como também foi possível encontrar um modelo de machine learning que respondia a pergunta inicial de "Nesta condição experimental, com estes valores de expressões gênicas e população de células, existira ao menos uma via metabólica sendo ativada?" com 99,69% de certeza. 
### Agradecimentos
Gostaria de agradecer imensamente a Alura, aos professores, a Vanessa e a comunidade. Sem algum de vocês nada disso seria possível. Este foi o meu primeiro contato com o mundo da ciência de dados e aprendi muita coisa nova e interessante, com certeza sou uma pessoa diferente do que era antes de iniciar a imersão. Gostaria de mergulhar cada vez mais fundo no universo do data science e machine learning, pois tenho total consciência que isto é apenas o começo de uma grande jornada de aprendizado, que seria muito bem aproveitada com a premiação desta imersão.
