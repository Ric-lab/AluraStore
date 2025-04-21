# 📊 Análise de Vendas - AluraStore

Este repositório contém uma análise exploratória de dados de vendas da AluraStore, focando no desempenho de quatro lojas diferentes. O objetivo do projeto é identificar padrões de vendas, avaliar o desempenho individual de cada loja e fornecer recomendações estratégicas baseadas nos dados.

## 📝 Visão Geral do Projeto

A análise utiliza dados de vendas de quatro arquivos CSV distintos, cada um representando uma loja da AluraStore. O notebook Jupyter (`Análise_AluraStore.ipynb`) realiza as seguintes etapas:

1.  **Importação e Consolidação:** Carrega os dados das quatro lojas e os une em um único DataFrame para análise comparativa.
2.  **Análise Exploratória de Dados (EDA):** Investiga diversas métricas para entender o comportamento das vendas e o desempenho das lojas.
3.  **Visualização de Dados:** Cria gráficos para ilustrar as descobertas e facilitar a compreensão dos resultados.
4.  **Conclusões e Recomendações:** Resume os principais insights e sugere ações estratégicas com base na análise.

## ✨ Análises Realizadas

*   **Faturamento e Vendas por Categoria:** Análise do total vendido e da quantidade de itens por categoria em cada loja.
*   **Ticket Médio:** Cálculo do valor médio gasto por compra em cada loja e categoria.
*   **Avaliação Média:** Análise da satisfação do cliente com base nas avaliações das compras por loja.
*   **Frete Médio:** Verificação do custo médio de frete por loja.
*   **Produtos Mais e Menos Vendidos:** Identificação dos produtos com maior e menor volume de vendas em cada loja.
*   **Análise de Pareto (80/20):**
    *   Categorias de produtos que representam 80% do faturamento em cada loja.
    *   Estados que concentram 80% das compras totais.
    *   Tipos de parcelamento mais comuns que representam 80% das compras.
*   **Análise Geográfica:** Ranking de compras por estado.
*   **Formas de Pagamento:** Identificação dos tipos de pagamento mais utilizados e análise da distribuição do parcelamento.
*   **Score de Desempenho das Lojas:** Cálculo de um score ponderado para cada loja, utilizando métricas normalizadas (Faturamento, Avaliação Média, Ticket Médio, Frete Médio, % de Categorias Não Rentáveis) para comparar o desempenho geral.
*   **Visualizações:** Gráficos de Pareto, Pizza, Radar e Barras para apresentar os resultados de forma clara.

## 💾 Fonte dos Dados

Os dados utilizados neste projeto foram fornecidos como parte do **Challenge 1 - Data Science da Alura Latam**. Eles estão divididos em quatro arquivos CSV, disponíveis nos seguintes links:

*   `loja_1.csv`: [https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_1.csv](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_1.csv)
*   `loja_2.csv`: [https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_2.csv](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_2.csv)
*   `loja_3.csv`: [https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_3.csv](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_3.csv)
*   `loja_4.csv`: [https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_4.csv](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science/refs/heads/main/base-de-dados-challenge-1/loja_4.csv)

## 🛠️ Tecnologias Utilizadas

*   **Python 3**
*   **Pandas:** Para manipulação e análise de dados.
*   **Matplotlib:** Para visualização de dados.
*   **Numpy:** Para operações numéricas (utilizado implicitamente pelo Pandas e Matplotlib).
*   **Scikit-learn:** Especificamente `MinMaxScaler` para normalização dos dados no cálculo do score.
*   **Jupyter Notebook:** Para desenvolvimento e apresentação da análise.

## 🚀 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    cd seu-repositorio
    ```
2.  **Instale as dependências:**
    ```bash
    pip install pandas matplotlib scikit-learn jupyter
    ```
3.  **Execute o Jupyter Notebook:**
    ```bash
    jupyter notebook Análise_AluraStore.ipynb
    ```
    Isso abrirá o notebook no seu navegador, onde você poderá executar as células de código para reproduzir a análise.

## 💡 Principais Descobertas e Conclusão

A análise revelou informações importantes sobre as vendas e o desempenho das lojas AluraStore:

*   **Categorias Líderes:** Eletrônicos, Eletrodomésticos e Móveis são responsáveis pela maior parte do faturamento (princípio de Pareto aplicado por loja).
*   **Concentração Geográfica:** Os estados das regiões Sul e Sudeste (especialmente SP, RJ, MG, RS, PR) concentram a grande maioria das compras (cerca de 80%).
*   **Pagamento Preferencial:** O Cartão de Crédito é a forma de pagamento dominante, respondendo por aproximadamente 75% das transações.
*   **Parcelamento:** Pagamentos em 1x são os mais comuns, e até 4 parcelas concentram cerca de 80% das compras parceladas.
*   **Desempenho das Lojas:**
    *   As lojas 2 e 3 apresentaram os melhores desempenhos gerais, com bons scores combinando faturamento, avaliação e eficiência (frete, ticket médio).
    *   A loja 1 teve um desempenho bom, mas inferior às lojas 2 e 3.
    *   A loja 4 demonstrou consistentemente o pior desempenho em várias métricas, resultando no menor score geral.

**Recomendação Estratégica:**

Com base nos dados, recomenda-se **focar os esforços nas categorias e regiões de maior retorno** (eletrônicos, eletrodomésticos, móveis; Sul/Sudeste) e otimizar as opções de pagamento e parcelamento via cartão de crédito. Dada a performance significativamente inferior, sugere-se **avaliar o fechamento ou uma reestruturação profunda da Loja 4**, realocando recursos para as lojas de melhor desempenho (Loja 2 e Loja 3).

---
