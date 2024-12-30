



# Projeto Final: Dashboard de Vendas B2B | SoulCode Embraer Social Tech Careers

![aviao](https://github.com/user-attachments/assets/4192fa75-e86f-4f58-88a6-792d65c9ab2a)

## Visão Geral

Este projeto tem como objetivo desenvolver um dashboard simples e intuitivo para análise de dados de vendas B2B (Business-to-Business), demonstrando a capacidade de utilizar os recursos do Google Cloud Platform (GCP) para o armazenamento, processamento e análise de dados, e a criação de visualizações com o Power BI. A base de dados utilizada para este projeto é fictícia, contendo informações sobre vendas de diferentes produtos para clientes em diversas regiões do Brasil.

A motivação principal é apresentar um caso prático de como os conceitos de Data Analytics e Business Intelligence podem ser aplicados, desde a extração dos dados até a visualização final. Um dos principais desafios é lidar com dados em formato CSV que foram distribuídos em múltiplos arquivos, além da necessidade de tratar inconsistências como valores ausentes, duplicidades e problemas de codificação. Para superar essas dificuldades, foi desenvolvido um pipeline ETL completo.

Através deste dashboard, serão explorados diversos aspectos das vendas, como:

*   Volume total de vendas por região.
*   Receita total por setor.
*   Quantidade de vendas por categoria de produto.
*   Desempenho individual dos vendedores (valor total vendido).
*   Produtos mais vendidos.

## Etapas do Projeto

### Etapa 1: Armazenamento Inicial

1.  **Google Cloud Storage (GCS):**
    *   Criação de um bucket no Google Cloud Storage para o armazenamento da base de dados fornecida.
    *   Organização dos dados brutos em uma pasta nomeada "dados brutos" dentro do bucket.
2.  **Google Cloud SQL (MySQL):**
    *   Criação de uma instância do MySQL no Google Cloud SQL.
    *   Transferência dos dados do GCS para o banco de dados MySQL, que será utilizado para explorar e manipular os dados de forma estruturada.
3.  **Modelo Entidade-Relacionamento (MER):**
    *   Criação e entrega do Modelo Entidade-Relacionamento (MER) que representa a estrutura da base de dados no MySQL. 

### Etapa 2: Processamento de Dados no Google Colab

1.  **Google Colab Notebook:**
    *   Desenvolvimento de um notebook no Google Colab para a realização do processo de Extração, Transformação e Carga (ETL).
    *   Extração dos dados, podendo ser feita a partir do bucket no Google Cloud Storage, do banco relacional no Google Cloud SQL ou ambos. A extração dos dados é feita de forma automatizada, utilizando as bibliotecas do Python para o acesso aos arquivos.
2.  **Transformação de Dados:**
    *   Manipulação dos dados para atender às perguntas do case, incluindo:
        *   Tratamento de valores ausentes (preenchidos com a média em colunas numéricas ou com "Desconhecido" em colunas de texto).
        *   Remoção de linhas duplicadas para garantir a integridade dos dados.
        *   Padronização de colunas de texto para garantir a consistência das informações.
        *   Criação de novas colunas para análises específicas.
        *   Consolidação de informações em tabelas estruturadas.
3.  **Documentação do Código:**
    *   Documentação clara e concisa de todo o código, com comentários explicativos em cada etapa do processo.
    *   O código do notebook pode ser acessado https://colab.research.google.com/drive/1rdUnGTt04WkG6Vl5bG84OYFOqLQDu1Cz .
   

### Etapa 3: Carregamento de Dados Tratados

1.  **Google BigQuery:**
    *   Carregamento dos dados transformados no Google BigQuery, usando o comando `bq load`.
    *   Criação de novas tabelas e/ou colunas baseadas em análises e agregações realizadas no Google Colab. Os dados serão disponibilizados na plataforma para a criação do dashboard.
2.  **Google Cloud Storage:**
    *   Carregamento dos dados transformados no Google Cloud Storage, criando novos arquivos CSV em um diretório nomeado `dados_tratados/`, para uso em outras plataformas ou projetos.

### Etapa 4: Visualização dos Dados

1.  **Power BI:**
    *   Criação do dashboard utilizando o Power BI, com base nos dados transformados e carregados no Google BigQuery. O Power BI foi escolhido pela sua flexibilidade e facilidade de visualização dos dados.
    *   Visualização de dados para os seguintes pontos de análise:
        *   Volume total de vendas por região.
        *   Receita total por setor.
        *   Quantidade de vendas por categoria de produto.
        *   Desempenho individual dos vendedores (valor total vendido).
        *   Produtos mais vendidos.
    *   O dashboard do PowerBI pode ser acessado https://drive.google.com/file/d/1JQggJ9RabiSaQ0iXPrsDsFHmCZw6WLDi/view .

## Tecnologias Utilizadas

*   **Google Cloud Platform**
    *   Google Cloud Storage
    *   Google Cloud SQL (MySQL)
    *   Google BigQuery
*   **Google Colab**
*   **Python** (com bibliotecas Pandas, google-cloud-storage e google-cloud-bigquery)
*   **Microsoft Power BI**

## Próximos Passos

*   Análise dos resultados no dashboard e elaboração de insights e recomendações para o negócio.
*   Aprimoramento do dashboard com novos indicadores e funcionalidades.
*   Explorar a possibilidade de integrar o BigQuery com o PowerBI para atualizações automáticas do dashboard.

## Considerações Finais

Este projeto demonstra a capacidade de utilizar os recursos do Google Cloud para o armazenamento, processamento e análise de dados de vendas B2B, e como criar visualizações interativas com o Power BI. O desenvolvimento do projeto nos permitiu explorar diversas tecnologias e conceitos de Data Analytics, e os resultados obtidos reforçam a importância de uma análise de dados estruturada para a tomada de decisões de negócio.

A experiência com Python para a automatização do processo ETL e o uso do Power BI para visualização e análise de resultados mostra que essas ferramentas são ideais para um profissional que deseja lidar com dados e apresentar informações de forma clara e concisa.

https://www.linkedin.com/in/jefferson-alveti/
