# SoulCode | Embraer SOCIAL TECH CAREERS 

Projeto Final: Dashboard de Vendas B2B

Visão Geral

Este projeto tem como objetivo desenvolver um dashboard simples e intuitivo para análise de dados de vendas B2B (Business-to-Business). Através deste dashboard, serão explorados diversos aspectos das vendas, como volume total por região, receita por setor, quantidade de vendas por categoria de produto, desempenho individual dos vendedores e os produtos mais vendidos.

Etapas do Projeto
Etapa 1: Armazenamento Inicial

Google Cloud Storage:

Criação de um bucket no Google Cloud Storage para o armazenamento da base de dados fornecida.

Organização dos dados brutos em uma pasta nomeada "dados brutos" dentro do bucket.

Google Cloud SQL (MySQL):

Criação de uma instância do MySQL no Google Cloud SQL.

Transferência dos dados do Google Cloud Storage para o banco de dados MySQL.

Modelo Entidade-Relacionamento (MER):

Criação e entrega do Modelo Entidade-Relacionamento (MER) que representa a estrutura da base de dados no MySQL.

Etapa 2: Processamento de Dados no Google Colab

Google Colab Notebook:

Desenvolvimento de um notebook no Google Colab para a realização do processo de Extração, Transformação e Carga (ETL).

Extração dos dados, podendo ser feita a partir do bucket no Google Cloud Storage, do banco relacional no Google Cloud SQL ou ambos.

Transformação de Dados:

Manipulação dos dados para atender às perguntas do case, incluindo:

Tratamento de valores ausentes.

Criação de novas colunas.

Consolidação de informações em tabelas estruturadas.

Documentação do Código:

Documentação clara e concisa de todo o código, com comentários explicativos em cada etapa do processo.

Etapa 3: Carregamento de Dados Tratados

Google BigQuery:

Carregamento dos dados transformados no Google BigQuery.

Criação de novas tabelas e/ou colunas baseadas em análises e agregações realizadas no Google Colab.

Google Cloud Storage:

Carregamento dos dados transformados no Google Cloud Storage, criando novos arquivos e pastas para dados tratados.

Etapa 4: Visualização dos Dados

Power BI:

Criação do dashboard utilizando o Power BI, com base nos dados transformados e carregados no Google BigQuery.

Visualização de dados para os seguintes pontos de análise:

Volume total de vendas por região.

Receita total por setor.

Quantidade de vendas por categoria de produto.

Desempenho individual dos vendedores (valor total vendido).

Produtos mais vendidos.

Tecnologias Utilizadas

Google Cloud Platform

Google Cloud Storage

Google Cloud SQL (MySQL)

Google BigQuery

Google Colab

Python

Microsoft Power BI

Próximos Passos

Análise dos resultados no dashboard e elaboração de insights e recomendações para o negócio.

Possível aprimoramento do dashboard com novos indicadores e funcionalidades.

Considerações Finais

Este projeto demonstra a capacidade de utilizar os recursos do Google Cloud para o armazenamento, processamento e análise de dados de vendas B2B, bem como a criação de visualizações com o Power BI. A documentação e o código desenvolvidos representam um aprendizado prático sobre os conceitos de Data Analytics e Business Intelligence.
