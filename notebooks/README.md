## Orçamentista
## Como orçamentista, eu gostaria de um previsão do orçamento da casa denominada "Projeto 4" em reais.

R: 

A previsão em reais se encontra no notebook_orçamentista (localizado em notebooks\notebook_orçamentista.ipynb), juntamente dos comentários que explicam partes do processo.

## Engenheiro Responsável
## Como engenheiro responsável pelo projeto, eu gostaria de ter a documentação completa do método usado para chegar ao valor previsto para o "Projeto 4", incluindo cálculos.

R: 

Respondendo diretamente a historia do engenheiro responsavel, vou passar aqui alguns pontos para um melhor entendimento dos métodos:

A princípio o código do notebook está documentado em sua maior parte, nas quais acredito que são necessárias para entendimento geral de código em si.
os cálculos foram básicos, não utilizei de nenhuma ferramenta milaborante, eu apenas fiz uma regressão linear com com os dados trabalhados das amostras, utilizei A área construída para relacionar com o valor total do projeto. O maior trabalho foi conseguir buscar esses dados e limpar eles da melhor forma para conseguir ao menos tentar tirar um número viável. Utilizei a lógica do terreno para entender se fazia sentido os preços serem alterados somente por ser "sobrado" e "térrea" e me pareceu que sim.


## Gerente comercial da conta do cliente
## Como gerente comercial da conta do cliente do "Projeto 4", eu gostaria de ter uma base estatística para indicar o quão aproximado o valor estipulado está da realidade, e no caso de variação, quanto esse valor pode variar.

R:

Se tirarmos como base os resultados do modelo, ele pode fornecer uma avaliação estatística da precisão da estimativa de custo para o Projeto 4. O score do modelo, calculado como 0.903, indica a capacidade do modelo de prever o custo total do projeto com base na área construída, lógica utilizada para a regressão.

A previsão do valor total para o Projeto 4 é de R$ 995.639,59. Mas é bem importante destacar que é uma previsão estimativa e deve haver variações com o projeto real. A gente consegue compreender mais se calcular a margem de erro ou intervalo de confiança. Isso permite que nós indiquemos o quão próxima a estimativa está da realidade e quanto pode variar.

E pra finalizar, apesar do modelo fornecer uma estimativa útil de custo do Projeto 4, é necessário reforçar que todas as previsões estão sujeitas a alguma incerteza.


## Responsável pela Gestão de risco de projetos
## Como responsável pela gestão de risco de projetos, eu gostaria de entender o risco implícito nessa previsão, indicando o que pode impactar em outliers ou variações acima do previsto.

R:

O modelo de regressão linear utilizado pode não capturar por completo a complexidade do de todo o processo de orçamentação de projetos de construção. Ele pode não levar em conta variáveis importantes ou não linearidades que existem nos dados, além de que o modelo foi treinado com base em um conjunto limitado de dados históricos. Se esses dados não forem representativos o suficiente ou não cobrirem todas as possíveis situações, a previsão pode ser imprecisa.

Se quisermos levar em consideração uma abordagem realista para a gestão de riscos em projetos, ela envolve estar ciente das limitações e preparo do modelo para lidar com a incerteza do processo de orçamentação de projetos. Isso pode incluir realizar análises de sensibilidade e a talvez implementação de planos de mitigação de riscos.


## Explicação da motivação de escolha das libs e frameworks. Uma explicação sobre a estrutura do projeto também será bem vinda.

R:

pandas, numpy, matplotlib, scikit-learn. Esses foram as principais libs que utilizei pra estruturar o projeto. Quando eu quis fazer uma regressão linear eu optei por elas por serem mais coerentes com o meu objetivo. tem outras libs importadas mas não foram usadas necessáriamente, eu estava fazendo teste para ver quais seriam os melhores para utilizar no fim.

Optei também por realizar algumas operações manualmente devido a natureza específica do projeto. Por exemplo, a limpeza e transformação dos dados foram feitas manualmente em algumas etapas para lidar com requisitos específicos do conjunto de dados.

Quanto à estrutura do projeto, eu segui uma abordagem modular, com diferentes partes do código organizadas em funções e módulos separados para facilitar a manutenção e a reutilização do código. Cada etapa do processo, desde a importação dos dados até a análise dos resultados, é tratada em um bloco de código separado que posteriormente foi adicionado a uma celula só, mas os blocos ainda existem se observar bem, isso facilita a compreensão do fluxo de trabalho e a identificação de possíveis melhorias além de não me perder o tempo inteiro.
