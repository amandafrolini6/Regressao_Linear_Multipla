# 📊 Regressão Linear Múltipla — Previsão de Preços de Imóveis

Projeto de Machine Learning desenvolvido em Python que aplica **Regressão Linear Simples** e **Regressão Linear Múltipla** para prever o preço de imóveis com base no dataset público **King County House Sales** (`kc_house_data.csv`).

---

## 🎯 Objetivo

Comparar o desempenho dos dois modelos de regressão e demonstrar, na prática, que considerar múltiplas variáveis (quartos, banheiros, área, andares, etc.) resulta em previsões muito mais precisas do que usar apenas uma variável isolada.

---

## 📁 Estrutura do Projeto

```
Regressao_Linear_Multipla/
│
├── regrecao_multipla.ipynb   # Notebook principal com todo o código e análise
├── kc_house_data.csv         # Dataset com dados reais de venda de imóveis
└── README.md                 # Este arquivo
```

---

## 🗂️ Sobre o Dataset

O arquivo `kc_house_data.csv` contém dados reais de vendas de imóveis no condado de King (Seattle, EUA). Cada linha representa uma casa vendida, com as seguintes colunas utilizadas no projeto:

| Coluna | Descrição |
|---|---|
| `price` | Preço de venda da casa (variável alvo — o que queremos prever) |
| `bedrooms` | Número de quartos |
| `bathrooms` | Número de banheiros |
| `sqft_living` | Área útil da casa em pés quadrados |
| `sqft_lot` | Área do terreno em pés quadrados |
| `floors` | Número de andares |
| `condition` | Condição geral do imóvel (1 a 5) |
| `yr_built` | Ano de construção |
| `yr_renovated` | Ano da última reforma (0 se nunca reformada) |

---

## 🧠 Conceitos Abordados

### Regressão Linear Simples
Usa **apenas uma variável** para prever o preço. Por exemplo: prever o preço só com base na área da casa. É simples, mas limitada — o preço de uma casa depende de muito mais fatores.

### Regressão Linear Múltipla
Usa **várias variáveis ao mesmo tempo** para fazer a previsão. Combina quartos, banheiros, área, condição do imóvel, etc. Isso gera um modelo mais completo e preciso.

A equação do modelo é:

```
Preço = β₀ + β₁·quartos + β₂·banheiros + β₃·área + β₄·andares + ...
```

Onde cada **β (beta)** é um peso que o modelo aprende automaticamente.

---

## ⚙️ Metodologia

O projeto implementa os modelos **do zero**, sem usar bibliotecas prontas de Machine Learning (como Scikit-learn), utilizando apenas **NumPy** e **Pandas**. O cálculo é feito pela **Equação Normal**:

```
β = (XᵀX)⁻¹ · Xᵀ · y
```

**Passo a passo:**

1. Leitura e tratamento do dataset com NumPy e Pandas
2. Separação das variáveis preditoras (X) e variável alvo (y = preço)
3. Adição da coluna de intercepto (β₀)
4. Cálculo dos coeficientes via Equação Normal
5. Previsão do preço para casas de teste
6. Comparação entre o preço real e o previsto

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **NumPy** — operações matemáticas e matriciais
- **Pandas** — leitura e manipulação do dataset
- **Jupyter Notebook** — ambiente de desenvolvimento interativo

---

## ▶️ Como Executar

**Pré-requisitos:** Python 3 instalado com as bibliotecas NumPy e Pandas.

```bash
# 1. Clone o repositório
git clone <url-do-repositorio>
cd Regressao_Linear_Multipla

# 2. Instale as dependências (se necessário)
pip install numpy pandas jupyter

# 3. Abra o notebook
jupyter notebook regrecao_multipla.ipynb
```

Execute as células na ordem para ver os resultados de cada modelo.

---

## 📈 Resultados

O modelo de **Regressão Linear Múltipla** apresentou previsões significativamente mais próximas dos preços reais em comparação à Regressão Linear Simples, confirmando que o preço de um imóvel é determinado pela combinação de múltiplos fatores e não por uma única característica isolada.

---

## 📌 Conclusão

A Regressão Linear Múltipla é a abordagem mais adequada para este problema. Ao considerar simultaneamente diversas características do imóvel, o modelo captura melhor a complexidade do mercado imobiliário, resultando em maior precisão e melhor ajuste aos dados reais.

---

> Projeto desenvolvido para fins acadêmicos — Fatec Jahu | Desenvolvimento de Software Multiplataforma
