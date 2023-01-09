<h1 align="center"> Fórmula 1 </h1>

<h2 align="center"> Construção de pipelines com o Azure Data Factory para ETL de dados reais da Fórmula 1, utilizando Azure Databricks, Spark Core, PySpark e Spark SQL, com posterior visualização dos dados no Power BI. </h2>

<h3> :arrow_forward: Status do Projeto: </h3> :white_check_mark: Concluído :white_check_mark: 

<h3> :hammer: Tecnologias do Projeto: </h3>

- `PySpark`
- `SQL`
- `Azure Cloud (Databricks, Data Factory, Data Lake)`
- `Power BI`

<h3>:warning: Ferramentas Necessárias: </h3>

- `É necessário possuir uma conta no Microsoft Azure para ter acesso aos serviços`
- `Power BI`

<h3>:clipboard: Descrição do Projeto: </h3>

<p align="justify">
Neste projeto, por meio do Azure Data Factory, eu construí pipelines para extração, tratamento e loading de dados reais da maior competição de automobilismo do mundo - a Fórmula 1. Através de notebooks do Databricks, utilizei comandos de PySpark e Spark SQL para tratar e preparar todos os dados necessários para sua visualização posterior no Power BI. Para armazenamento dos dados, eu montei três camadas (de acordo com o tipo de dado disponível) no Data Lake Gen2, nas quais, utilizando o formato delta, pude construir um delta lake para armazená-los. 
Foram utilizados dados desde a primeira corrida até a de 18/04/2021, conforme o dataset encontrado e extraído. Ao final, eu linkei as tabelas criadas no Databricks com um arquivo no Power BI, onde foi possível extrair diversos insights a respeito de todas as corridas, equipes e pilotos, desde a primeira, em 1950, até a corrida de 18/04/2021.

<p align="justify">
Disponibilizei os notebooks em formato .dbc (para serem visualizados no Databricks ou outro framework compatível) e .zip contendo arquivos .py (para serem lidos em alguma IDE utilizando Python). O arquivo "incremental_load_data.zip" contém o dataset divididos em 3 pastas contendo arquivos JSON e CSV: 2021-03-21, contendo todas as corridas até essa data; 2021-03-28, com a corrida dessa data; 2021-04-18, também com a corrida dessa data. Por fim, meus dashboards podem ser visualizados no arquivo "DashBoard F1.pbix".
