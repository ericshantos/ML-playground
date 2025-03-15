# Clustering de Clientes para Marketing com K-means

Este repositório contém um estudo de caso sobre segmentação de clientes utilizando o algoritmo K-means. O objetivo é agrupar clientes de uma empresa de varejo com base em suas características, como idade, renda anual e pontuação de gastos, para auxiliar em campanhas de marketing mais direcionadas e eficientes.

## Descrição do Projeto

O projeto é composto por um notebook Jupyter (`clustering_client_marketing.ipynb`) que realiza a análise de dados, pré-processamento, clusterização e visualização dos resultados. O conjunto de dados utilizado é o **Mall_Customers.csv**, que contém informações sobre clientes de um shopping, incluindo:

- **CustomerID**: Identificador único do cliente.
- **Gender**: Gênero do cliente (Masculino/Feminino).
- **Age**: Idade do cliente.
- **Annual Income (k$)**: Renda anual do cliente em milhares de dólares.
- **Spending Score (1-100)**: Pontuação de gastos do cliente, onde 1 indica baixo gasto e 100 indica alto gasto.

### Estrutura do Projeto

1. **Carregamento dos Dados**:
   - O conjunto de dados é carregado a partir do Kaggle utilizando a biblioteca `kagglehub`.
   - Uma análise inicial dos dados é realizada para entender a estrutura e a qualidade dos dados.

2. **Análise Exploratória**:
   - Verificação de valores nulos e duplicados.
   - Análise de correlação entre as variáveis numéricas.
   - Visualização das distribuições e relações entre as variáveis.

3. **Pré-processamento**:
   - Normalização dos dados para garantir que todas as variáveis tenham a mesma escala.
   - Remoção de variáveis irrelevantes, como o `CustomerID`.
   - Tratamento de outliers utilizando o método **Local Outlier Factor (LOF)**.

4. **Clusterização com K-means**:
   - Aplicação do método do cotovelo para determinar o número ideal de clusters.
   - Execução do algoritmo K-means para agrupar os clientes com base em sua renda anual e pontuação de gastos.
   - Visualização dos clusters formados e dos centróides.

5. **Avaliação dos Clusters**:
   - Cálculo do índice de silhueta para avaliar a qualidade dos clusters formados.

## Requisitos

Para executar o notebook, é necessário ter instalado as seguintes bibliotecas Python:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `kagglehub`

Você pode instalar todas as dependências utilizando o seguinte comando:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub
```

## Como Executar

1. Clone este repositório:

```bash
git clone https://github.com/ericshantos/ML-playground.git
```

2. Navegue até o diretório do projeto:

```bash
cd clustering/client-marketing
```

3. Execute o notebook Jupyter:

```bash
jupyter notebook clustering_client_marketing.ipynb
```

## Resultados

O algoritmo K-means foi capaz de identificar 5 clusters distintos de clientes com base em sua renda anual e pontuação de gastos. A visualização dos clusters mostra a distribuição dos clientes e os centróides de cada grupo. O índice de silhueta médio foi de **0.55**, indicando uma boa separação entre os clusters.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo [LICENSE](../../LICENSE) para mais detalhes.

## Agradecimentos

- O conjunto de dados foi obtido a partir do Kaggle: [Customer Segmentation Tutorial in Python](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python).
- Agradecimentos à comunidade de ciência de dados por fornecer ferramentas e recursos valiosos.