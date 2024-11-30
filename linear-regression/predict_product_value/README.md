
# 🛠️ Prevendo o Preço de Vendas com Base na Quantidade Vendida

Este projeto foi desenvolvido para criar e avaliar um modelo de regressão linear simples. 
O objetivo principal é prever o **preço de venda** de um produto com base na sua **quantidade vendida**. 📈

---

## 📝 Descrição do Projeto

Dado um conjunto fictício de dados sobre vendas, este projeto explora o uso de regressão linear para entender e prever a relação entre **quantidade vendida** e **preço de venda**. 
Isso inclui desde a análise exploratória até a implementação de um modelo preditivo e a avaliação de sua performance. 

Os passos principais foram:
1. **Carregamento e visualização dos dados** 📊
2. **Criação do modelo de regressão linear simples** 🧮
3. **Treinamento e avaliação do modelo** 🏋️‍♂️
4. **Predições com novos dados** 🔮

---

## 🔍 Conjunto de Dados

### Estrutura dos Dados:
| Quantidade Vendida | Preço de Venda (R$) |
|---------------------|---------------------|
| 1                   | 50                  |
| 2                   | 90                  |
| 3                   | 130                 |
| ...                 | ...                 |
| 10                  | 410                 |

---

## 📂 Etapas de Desenvolvimento

### 1️⃣ Carregamento dos Dados
Os dados foram carregados utilizando o **Pandas**, permitindo manipulação e exploração simples.

### 2️⃣ Visualização dos Dados
Criamos gráficos de dispersão para entender a relação entre as variáveis e identificar padrões.

### 3️⃣ Criação do Modelo
Utilizamos a fórmula clássica da regressão linear:

> \( Y = aX + b \)

Onde:
- \( Y \): **Preço de Venda** (variável dependente)
- \( X \): **Quantidade Vendida** (variável independente)
- \( a \): Coeficiente angular
- \( b \): Intercepto

O modelo foi implementado usando **scikit-learn**.

### 4️⃣ Treinamento e Avaliação
- **Métricas utilizadas**: Erro Médio Absoluto (MAE), Erro Quadrático Médio (MSE) e R².
- **Bibliotecas**: `sklearn.metrics`.

### 5️⃣ Previsões
Após o treinamento, realizamos previsões para novas quantidades vendidas, como, por exemplo, **11 unidades**.

---

## 🧰 Tecnologias Utilizadas

- **Python** 🐍
- **Pandas** para manipulação de dados
- **Matplotlib** e **Seaborn** para visualização de dados
- **Scikit-learn** para treinamento e avaliação do modelo

---

## 📈 Resultados Obtidos

- A linha de regressão foi ajustada adequadamente aos dados.
- O modelo apresentou métricas de avaliação satisfatórias, demonstrando sua capacidade de prever preços baseados na quantidade vendida.

### Exemplo de Previsão:
Com base na quantidade vendida de **11 unidades**, o modelo previu um preço de venda de aproximadamente **R$450,00**.

---

## 🤝 Contribuições

Sinta-se à vontade para explorar, melhorar e sugerir alterações neste projeto! Clone o repositório e experimente. 😄

---

## 🛡️ Licença

Este projeto está sob a licença MIT - veja o arquivo LICENSE para mais detalhes.

---

🚀 **Divirta-se explorando os conceitos de regressão linear!** ✨
