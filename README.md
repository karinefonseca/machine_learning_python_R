# Machine Learning

Neste repositório estão os projetos referentes à Machine Learning, tanto em Python quanto em R. Aqui, faço um breve resumo de cada um deles. 

## Análise Exploratória - Mental_Health

Neste trabalho são introduzidos alguns conceitos e comandos para a realização da análise exploratória de dados em R. Faço a visualização geral do DataFrame, onde o mesmo posui 27 atributos e 1259 instâncias, destes atributos 26 são do tipo ch (character) e 1 do tipo num. Verifico os valores de máximo, mínimo, média e mediana da coluna Age, onde percebe-se que o mesmo possui uma série de outliers que precisarão de tratamento. Faço também a plotagem de histogramas e boxplots, assim como a matriz de correlação. Por fim verifico missing.

## Classificação

### Abalone

Neste trabalho analiso os dados de https://archive.ics.uci.edu/ml/datasets/abalone. E faço a classificação utilzando Árvores de Decisão (Decision Trees).

O abalone é um molusco gastrópode pertencente à família Haliotidae e é encontrado sob a forma de diversas espécies em águas costeiras de quase todo o mundo. Por causa de seu uso como jóia e alimento,há duas espécies de abalone que se encontram em risco de extinção.

A idade é determinada cortando a casca através do cone, manchando-a e contando o número de anéis através de um microscópio. Outras medidas, mais fáceis de obter, são usadas para prever a idade.

Neste projeto, é determinada idade do abalone baseada em fatores físicos. Para fazer a classificação faço a categorização do atributo RINGS em "Old", "Adult" e "Young". (Somando 1.5 ao número de RINGS temos a idade do Abalone em anos).

### Labor

Neste trabalho analiso os dados de http://archive.ics.uci.edu/ml/datasets/Labor+Relations?ref=datanews.io e o artigo mencionado para o projeto está em http://ebot.gmu.edu/handle/1920/1622.

O projeto original, conforme a descrição do mesmo, teve como propósito "Software de aprendizagem de conceitos testando um método experimental para aprender descrições de conceitos em duas camadas. Os dados foram utilizados para aprender a descrição de um contrato aceitável e não aceitável. Os contratos não aceitáveis foram obtidos por meio de entrevistas com especialistas ou por meio de criação de exemplos similares, mas que não atendiam aos requisitos do contrato aceitável."


## Retenção de Clientes (Modelo de Predição de Churn) 

Este projeto, concebido durante o curso de Fundamentos de Machine Learning, tem como objetivo a comparação de diversos modelos para a predição de churn, uma métrica que indica a perda de clientes. O propósito primordial é a avaliação de conjuntos de dados para prever se um cliente tem probabilidade de abandonar a empresa.

Implementado utilizando a linguagem de programação Python, é realizada uma análise da relação entre as variáveis, seguida da seleção daquelas que possuem forte correlação com a saída dos clientes. Posteriormente, é conduzido o pré-processamento dos dados, sendo então aplicados os seguintes modelos: Regressão Logística, Árvore de Decisão, KNN (K-Nearest Neighbors), Bagging e Random Forest.

Ao término da análise, os resultados são avaliados utilizando métricas como acurácia, sensibilidade, precisão, eficiência e f1-score, as quais são contextualizadas com os aspectos de negócio. Esta análise permite a identificação do modelo mais adequado para embasar a tomada de decisão estratégica.
  
## Reconhecimento de Fala (Speech Recognition)

Este projeto, realizado durante o curso de Natural Language Processing: Machine Learning NLP In Python, representa uma aplicação prática da tecnologia de reconhecimento de fala. Utilizando a Google Speech Recognition API como ferramenta principal, o objetivo é realizar o reconhecimento e subsequente transcrição (Speech-to-Text) de áudios enviados, proporcionando uma experiência de comunicação mais acessível e eficiente.

A escolha da Google Speech Recognition API se dá pela sua reconhecida precisão e confiabilidade na transcrição de fala para texto, o que é essencial para garantir resultados de alta qualidade neste contexto. Além disso, a API oferece uma integração fluida com a linguagem de programação Python, permitindo uma implementação suave e eficaz do projeto.

A utilização da Google Speech Recognition API abre portas para uma ampla gama de aplicações práticas, desde assistentes virtuais inteligentes até sistemas de transcrição automatizada em tempo real para pessoas com deficiência auditiva.

## Redes Neurais

São utilizadas redes neurais em R (neuralnet()) para fazer a classificação de moluscos Abalone quanto a sua idade.

Para este projeto verifiquei o balanceamento das classes, a quantidade de instâncias em cada classe e fiz a comparação entre os resultados do modelo com e sem amostragem. 

Utilizando todo o dataset, o modelo prediz que todas as instâncias são da classe "adult". Comportamento este esperado tendo em vista o desbalanceamento. Com a amostragem, embora a acurácia tenha dimunído, o modelo acertou mais de cada classe. Assim optei por utilizar a amostragem.

## Regressão

Utilizei modelo de Regressão Linear em R (utilizando method lm) e Support Vector Machines com Kernel Linear (method svmLinear) também para a predição da idade do molusco Abalone. 

Fiz duas execuções de maneiras diferentes utilizando modelo linear (SVM com kernel linear e a própria regressão linear). Como esperado, ambos obtiveram RMSE por volta de 2.5,o que significa um desvio padrão de 2.5 dos valores reais. Para o caso do abalone, onde os valores são baixos, considero um resultado mediano para ruim.

## Competicação_Flai (8ª Competição de Machine Learning - Flai)
  
Neste projeto analiso o turnover (rotatividade) de profissionais de uma empresa. Primeiramente faço uma análise exploratória e pré-processamento dos dados e posterior comparação entre os modelos utilizando as métricas de acurácia, sensibilidade, precisão, eficiência e f1-score, seguindo as orientações encaminhadas aos participantes. Nessa competição obtive o 5º lugar da minha turma e 22º lugar geral. 

## Pre_Processamento

Neste trabalho analiso os dados de https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey que se trata de uma base de dados oriunda de uma pesquisa sobre a saúde mental e frequência de doenças mentais na área tech. Em um primeiro momento faço a análise exploratória, verificando o número de atributos e instâncias, analiso o atributo AGE onde percebe-se a presença de outliers que precisarão ser tratados. Verificação de missing, discretização do atributo AGE para três categorias "jovem", "jovem adulto" e "adulto" tanto pelo método frequency quanto pelo método interval. Padronização do atributo GENDER, amostragem e analise final.

