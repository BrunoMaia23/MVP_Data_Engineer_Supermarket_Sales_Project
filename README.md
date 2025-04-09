# MVP_Data_Engineer_Supermarket_Sales_Project

# Análise de Vendas e Otimização da Cadeia de Suprimentos em Supermercados

## Resumo do Projeto
Este projeto tem como objetivo analisar os dados de vendas de supermercados para auxiliar na definição de estratégias de marketing e na otimização da cadeia de suprimentos. Com base no dataset [Supermarket Sales - Kaggle](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales), foram utilizadas as camadas Bronze, Silver e Gold para processar, transformar e analisar os dados.

## Objetivos e Perguntas de Negócio
- **Objetivo:**  
  Investigar padrões de compra, identificar as linhas de produtos com maior faturamento e analisar a performance das filiais, visando otimizar campanhas de marketing e a logística de estoque.

- **Perguntas de Negócio:**  
  - Quais são as linhas de produtos com maior faturamento?  
  - Quais filiais e cidades geram mais vendas?  
  - Como as vendas variam por mês, ano e dia da semana?  
  - Qual o impacto dos métodos de pagamento e do perfil do cliente nas vendas?  
  - Qual a margem de lucro média por filial?

## Pipeline de Dados

### Camada Bronze
- **Descrição:** Ingestão dos dados brutos (CSV) e armazenamento em formato Parquet/Delta.
- **Arquivo(s):** `notebooks/01_bronze_layer.ipynb`

### Camada Silver
- **Descrição:** Processamento e transformação dos dados com limpeza, conversão de datas, criação de colunas derivadas e aplicação de arredondamentos.
- **Arquivo(s):** `notebooks/02_silver_layer.ipynb`

### Camada Gold
- **Descrição:** Agregações e análises utilizando consultas SQL para extrair insights que respondem às perguntas de negócio.
- **Arquivo(s):** `notebooks/03_gold_layer.sql`

## Resultados e Insights
- Inclua aqui um resumo dos principais resultados extraídos das análises, assim como evidências visuais (veja a pasta `evidencias/`).

## Como Executar o Projeto
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/Supermarket_Sales_Project.git
