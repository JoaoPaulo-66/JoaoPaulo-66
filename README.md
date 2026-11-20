# Olá, eu sou o João Paulo 👋

Analista de Dados em Belo Horizonte. Trabalho transformando bases bagunçadas em indicador que alguém usa para decidir alguma coisa.

Hoje atuo como Analista de Dados na Gnoq, com dados e BI. Antes disso, passei pela MSX International cuidando dos indicadores de NPS das marcas do grupo Stellantis, onde reformulei e automatizei a apuração de uma base de mais de 1 milhão de linhas. Atualmente curso a pós-graduação em AI Scientist na FIAP.

**Stack:** Power BI (DAX, Power Query, Service) · SQL · Python (pandas, scikit-learn) · Machine Learning · AWS (S3, Athena, Glue) · ETL · Modelagem de dados

---

## Projetos

### [nps-preditivo-ecommerce](https://github.com/JoaoPaulo-66/nps-preditivo-ecommerce)
Análise de NPS de 2.500 pedidos em e-commerce que mostrou algo contraintuitivo: o tempo total de entrega não tem relação com a nota (correlação 0,00), mas o atraso sobre o prazo prometido tem (-0,60). Isso muda a recomendação de "entregar mais rápido" para "prometer o prazo certo". A partir daí, um modelo que estima o risco de um cliente virar detrator antes de a pesquisa ser enviada (ROC-AUC 0,870 contra 0,500 do baseline) e um dashboard em Power BI de duas páginas, onde a área de atendimento escolhe o limiar de risco e vê na hora quantos clientes entram na fila de contato e quantos ficam de fora. O CSAT interno se mostrou descalibrado frente ao NPS real.
[Dashboard publicado](https://app.powerbi.com/view?r=eyJrIjoiMmUzNjhkY2UtYzNhZC00ODVlLTk1NTItZTAyNDFmMjI5NjI5IiwidCI6IjY1NTEwMzFhLWRlNTItNGY4MS04ODk3LWE4Zjg0MGY4MWU4MSJ9)

`Python` `scikit-learn` `Power BI` `DAX` `Power Query`

Os dois projetos abaixo formam uma série: o lakehouse construiu a base de dados na AWS, e o modelo de risco usou essa base para o Machine Learning. Juntos, mostram o ciclo completo, da ingestão bruta até o modelo interpretado.

### [brazil-literacy-risk](https://github.com/JoaoPaulo-66/brazil-literacy-risk)
Modelo de classificação que prevê o risco de uma criança do 2º ano não estar alfabetizada, usando o contexto do município e dados socioeconômicos da API do IBGE, para ajudar gestores públicos a priorizar onde agir. Base de 1,85 milhão de alunos extraída do lakehouse, 6 fontes de data leakage identificadas e tratadas, e validação agrupada por município. Comparação de 4 modelos com critério de escolha definido antes dos resultados, com a Regressão Logística escolhida pela explicabilidade. No nível do município, a taxa prevista teve correlação de 0,79 com a real em municípios nunca vistos pelo modelo.

`Python` `scikit-learn` `LightGBM` `SHAP` `KMeans` `AWS Athena` `API IBGE`

### [brazil-literacy-lakehouse](https://github.com/JoaoPaulo-66/brazil-literacy-lakehouse)
Lakehouse na AWS integrando seis bases públicas de alfabetização municipal, com ingestão batch e streaming, arquitetura em camadas bronze/silver/gold e 13 testes automatizados de qualidade. Mais de 4 milhões de registros processados, com custo total de infraestrutura abaixo de US$ 0,02.

`Python` `SQL` `AWS S3` `Athena` `Glue` `Kinesis Firehose` `Parquet`

---

## Onde me achar

[LinkedIn](https://linkedin.com/in/joaopaulorezendeoliveira)
