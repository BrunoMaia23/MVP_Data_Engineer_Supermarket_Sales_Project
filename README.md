# 🛒 MVP - Análise de Vendas de Supermercado com Databricks

## 📌 Tema
**Análise de Vendas e Otimização da Cadeia de Suprimentos em Supermercados**

## 🎯 Objetivo do Projeto
Investigar padrões de compra dos clientes a fim de:
- Auxiliar na definição de estratégias de marketing (promoções, segmentação, campanhas).
- Otimizar a gestão de estoque e logística com base no comportamento de vendas.

## ❓ Perguntas de Negócio
- Quais são as linhas de produtos com maior faturamento?
- Quais filiais e cidades geram mais vendas?
- Como variam as vendas por mês, ano e dia da semana?
- Qual o impacto dos métodos de pagamento nas vendas?
- Qual a margem de lucro média por filial?
- Há diferença no comportamento entre tipos de clientes (Member vs Normal) e entre gêneros?
- Qual é a avaliação média dos clientes para cada linha de produtos?

## 🗂️ Pipeline de Dados (Delta Lake)

### 🔹 Camada Bronze
- **Descrição:** Ingestão dos dados brutos (formato CSV) e salvamento em formato Parquet.
- **Operações:** Leitura dos dados com inferência de schema e visualização inicial para inspeção.

### 🔸 Camada Silver
- **Descrição:** Transformações e limpeza dos dados.
- **Operações:**
  - Conversão de datas e timestamps.
  - Criação de colunas derivadas: dia da semana, mês, ano, margem de lucro.
  - Padronização de nomes de colunas e arredondamentos.

### 🥇 Camada Gold
- **Descrição:** Agregações e análises analíticas com SQL.
- **Objetivo:** Responder diretamente às perguntas de negócio e extrair insights estratégicos.

---

## 📊 Principais Resultados

| Insight | Detalhes |
|--------|----------|
| **Produto mais lucrativo** | *Food and Beverages* (R$ 56.144,84 de faturamento) |
| **Cidade com maior receita** | *Naypyitaw* (R$ 110.568,71) |
| **Método de pagamento mais utilizado** | *Dinheiro (Cash)* |
| **Gênero com maior ticket médio** | *Feminino (Member)* |
| **Melhor dia para vendas** | *Sábado* |
| **Linha de produto com melhor avaliação** | *Food and Beverages* (Nota média: 7.11) |

---

🧠 Conclusão & Insights
A análise dos dados de vendas do supermercado revelou padrões valiosos de comportamento do consumidor e desempenho financeiro. Observamos que a linha de produtos "Food and Beverages" lidera em receita, enquanto a forma de pagamento "Ewallet" é amplamente preferida, indicando uma tendência crescente por transações digitais. A cidade com maior faturamento foi Naypyitaw, sugerindo maior poder aquisitivo ou concentração de consumo. Além disso, a margem de lucro variou significativamente entre os produtos, sendo essencial focar nos itens de maior retorno. Estes insights podem embasar decisões estratégicas de marketing, gestão de estoque e expansão comercial, maximizando o desempenho da operação.

---



## 🧪 Tecnologias Utilizadas
- Databricks
- Apache Spark (PySpark)
- SQL (Databricks SQL)
- Delta Lake
- Kaggle Datasets

---

**Schema Gold:** (branch: string, city: string, customer_type: string, gender: string, product_line: string, payment: string, gross_income: double, total: double, rating: double, quantity: int, unit_price: double, cost: double, date: date, day_of_week: string, month: string, year: int, profit_margin: double)
