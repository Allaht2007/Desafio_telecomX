# 📡 Telecom X - Análise de Evasão de Clientes (Churn)

## 📋 Sobre o Projeto
Este projeto foi desenvolvido como parte de um desafio técnico para a posição de **Analista de Dados na Telecom X**. O objetivo principal é analisar a base de dados de clientes da empresa para identificar padrões e fatores que contribuem para o *Churn* (cancelamento de serviços).

A empresa enfrenta um alto índice de cancelamentos e precisa entender os motivos para desenvolver estratégias de retenção eficazes.

---

## 🎯 Objetivos do Desafio
O projeto foi estruturado nas seguintes etapas, conforme os requisitos do desafio:

* **ETL (Extração, Transformação e Carga):**
    * Importação de dados brutos em formato JSON aninhado.
    * Normalização (achatamento) dos dados para estrutura tabular.
* **Limpeza e Tratamento de Dados:**
    * Identificação e remoção de dados inconsistentes (Churn vazio).
    * Conversão de tipos de dados (ex: `TotalCharges` de string para float).
    * Tratamento de valores nulos.
* **Engenharia de Atributos (Feature Engineering):**
    * Criação da coluna **Contas Diárias** (`Charges.Daily`) para refinar a análise de gastos.
* **Análise Exploratória de Dados (EDA):**
    * Visualização da distribuição de evasão.
    * Análise de variáveis categóricas (Contratos, Segurança Online, Pagamento).
    * Análise de variáveis numéricas (Gastos Mensais e Diários).
* **Análise de Correlação:**
    * Verificação estatística da relação entre variáveis numéricas e a evasão.

---

## 🛠 Tecnologias Utilizadas
O projeto foi desenvolvido em **Python** e pode ser executado no Google Colab ou Jupyter Notebook.

* **Pandas:** Manipulação e análise de dados.
* **NumPy:** Computação numérica.
* **Seaborn & Matplotlib:** Visualização de dados e gráficos estatísticos.
* **JSON:** Processamento do formato original dos dados.

---

## 📂 Estrutura dos Arquivos

* `TelecomX_Analise_Churn.ipynb`: Notebook com todo o código e relatórios.
* `TelecomX_Data.json`: Base de dados utilizada (necessária para rodar o código).
* `TelecomX_dicionario.md`: Documentação das variáveis do dataset.
* `README.md`: Documentação do projeto.

---

## 🚀 Como Executar

### Opção 1: Google Colab (Recomendado)
1.  Faça o upload do notebook `TelecomX_Analise_Churn.ipynb` no Google Colab.
2.  Faça o upload do arquivo de dados `TelecomX_Data.json` na aba de arquivos (lateral esquerda).
3.  Execute todas as células (**Runtime > Run all**).

---

## 📊 Principais Insights do Relatório
A análise revelou padrões críticos sobre o comportamento dos clientes:

* **Fator Contratual:** A modalidade "Month-to-month" é o maior ofensor, concentrando a maioria das evasões.
* **Sensibilidade ao Preço:** Clientes com churn positivo tendem a ter faturas mensais e diárias mais elevadas.
* **Serviços de Proteção:** A ausência de serviços adicionais, como *Online Security*, está fortemente correlacionada com a saída do cliente.
