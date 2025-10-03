# pipeline_elen_dados_vendas
Projeto de análise de dados e previsão de pipeline de vendas.


# Projeto: Pipeline e Análide de Dados de Vendas e Previsão de Churn

## 📝 Descrição

Este projeto realiza uma análise completa de um pipeline de vendas, utilizando um dataset público de e-commerce da Olist. O objetivo é organizar os dados vindos do CRM da Olist, limpar e estruturar os dados, extrair insights através de análise exploratória, e construir um modelo de Machine Learning para prever se um pedido será concluído com sucesso ('delivered') ou não. O projeto culmina em um dashboard interativo para visualização dos resultados.

Este trabalho foi desenvolvido como um estudo de caso prático, cobrindo o ciclo de vida de um projeto de dados, desde a coleta até a entrega dos resultados.

## 🎯 Objetivo de Negócio

O principal objetivo é entender os fatores que influenciam o sucesso de uma venda e criar um modelo preditivo baseado no ML de Regressão Logística que possa, com base nos dados iniciais de um pedido, estimar sua probabilidade de sucesso. Isso pode ajudar a empresa a:
* Identificar gargalos no processo de venda.
* Priorizar pedidos com maior risco de falha.
* Entender o perfil de clientes e produtos com maior taxa de sucesso.

## 🗃️ Fonte de Dados

Os dados utilizados foram obtidos do [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) disponível no Kaggle.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Bibliotecas de Análise:** Pandas, Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn (Logistic Regression)
* **Visualização/BI:** Looker Studio (Google Data Studio)
* **Versionamento:** Git e GitHub
* **Ambiente:** VS Code, Jupyter Notebook

## 📂 Estrutura do Projeto

O repositório está organizado da seguinte forma:

```
/meu_pipeline_vendas
|-- .gitignore
|-- README.md
|-- requirements.txt
|-- dados/
|   |-- olist_..._dataset.csv
|   |-- dados_para_dashboard.csv
|-- notebooks/
|   |-- 01-analise-exploratoria.ipynb
|-- dashboard/
|   |-- ![dash_pipeline_crm_vendas_modelo_preditivo](dash_pipeline_crm_vendas_modelo_preditivo.png)
```


## 🚀 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/SEU_USUARIO/meu_pipeline_vendas.git](https://github.com/SEU_USUARIO/meu_pipeline_vendas.git)
    cd meu_pipeline_vendas
    ```
2.  **Crie e ative um ambiente virtual:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Mac/Linux
    .\venv\Scripts\activate    # Windows
    ```
3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Execute o Notebook:**
    Abra o arquivo `notebooks/01-analise-exploratoria.ipynb` em um ambiente Jupyter (como o VS Code) e execute as células.

## ✨ Resultados

A análise exploratória revelou insights sobre o comportamento de compra por estado e a performance de diferentes categorias de produto.

O modelo de Regressão Logística treinado alcançou uma **acurácia de 98.85%** nos dados de teste, demonstrando eficácia na previsão de sucesso dos pedidos.

Um dashboard interativo foi criado para apresentar os principais KPIs e a performance do modelo.

**[Link para o Dashboard no Looker Studio](https://lookerstudio.google.com/reporting/7d9b56f4-889f-47dd-a31a-6a0658a12c59)**

![Screenshot do Dashboard](dash_pipeline_crm_vendas_modelo_preditivo.png)
