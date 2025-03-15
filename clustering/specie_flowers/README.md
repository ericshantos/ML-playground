# Clustering de Espécies de Flores com Base em Características Biológicas

Este repositório contém um estudo de caso sobre o agrupamento de espécies de flores com base em suas características biológicas, utilizando técnicas de aprendizado não supervisionado. O projeto foi desenvolvido em um notebook Jupyter.

## Visão Geral

O objetivo deste estudo é explorar e agrupar espécies de flores com base em suas características biológicas, como comprimento e largura das sépalas e pétalas. Utilizamos técnicas de análise exploratória de dados (AED), pré-processamento de dados, e algoritmos de clusterização como **PCA** (Principal Component Analysis) e **K-Means** para identificar padrões e estruturar os clusters.

## Conteúdo do Repositório

- **clustering_species_flowers.ipynb**: O notebook Jupyter que contém todo o código e análise.
- **README.md**: Este arquivo, que fornece uma visão geral do projeto.

## Dependências

Para executar o notebook, você precisará das seguintes bibliotecas Python:

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `scikit-learn`
- `kagglehub`

Você pode instalar todas as dependências usando o seguinte comando:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn kagglehub
```

## Metodologia

### 1. Carregamento de Dados
O conjunto de dados utilizado é o famoso **Iris Flower Dataset**, que contém 150 amostras de flores de íris, com quatro características cada: comprimento da sépala, largura da sépala, comprimento da pétala e largura da pétala.

### 2. Análise Exploratória de Dados (AED)
Realiza uma análise exploratória dos dados para entender a distribuição e a relação entre as variáveis. Isso incluiu a visualização de histogramas, boxplots, e gráficos de dispersão.

### 3. Pré-processamento de Dados
Os dados foram normalizados e outliers foram removidos para melhorar a qualidade do modelo.

### 4. Clusterização
Utiliza o algoritmo **K-Means** para agrupar as espécies de flores. Para reduzir a dimensionalidade dos dados, aplicamos o **PCA** (Principal Component Analysis).

### 5. Avaliação
Avalia a qualidade dos clusters utilizando o **Índice de Silhueta**.

## Resultados

- **Distribuições das variáveis**: As variáveis de pétalas mostraram-se mais eficazes para diferenciar as espécies.
- **Correlação entre variáveis**: Observei uma forte correlação entre o comprimento e a largura das pétalas.
- **Clusters**: O algoritmo K-Means foi capaz de identificar três clusters distintos, correspondentes às três espécies de flores.
- **Índice de Silhueta**: O índice médio da silhueta foi de **0.55**, indicando uma boa separação entre os clusters.

## Como Executar o Projeto

1. Clone este repositório:

```bash
git clone https://github.com/ericshantos/ML-playground.git
```

2. Navegue até o diretório do projeto:

```bash
cd clustering/species-flowers
```

3. Abra o notebook Jupyter:

```bash
jupyter notebook clustering_species_flowers.ipynb
```

4. Execute as células do notebook para reproduzir a análise.

## Licença

Este projeto está licenciado sob a **MIT License**. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.