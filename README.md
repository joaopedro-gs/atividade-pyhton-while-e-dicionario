# README - Arquivo de Contas e Saldos

Este documento descreve o arquivo `contas_saldos.csv` utilizado neste notebook para análises financeiras e manipulação de dados com a biblioteca Pandas.

## 📋 Descrição do Arquivo

O arquivo `contas_saldos.csv` contém informações estruturadas de contas de clientes e seus respectivos saldos financeiros. Ele serve como base para estudos de estatística descritiva, filtros e operações com DataFrames.

## 📊 Estrutura dos Dados

O arquivo é composto por duas colunas principais:

1. **`Conta`** (Numérico/Inteiro): Identificador único da conta bancária ou do cliente (ex: `1010`, `1020`, etc.).
2. **`Saldo`** (Numérico/Decimal): O saldo financeiro atual disponível na conta correspondente.

### Exemplo de Dados

| Conta | Saldo |
| :--- | :--- |
| 1010 | 1066.46 |
| 1020 | 1864.52 |
| 1030 | 2452.38 |

## 🛠️ Como Carregar os Dados em Python

Para ler e analisar este arquivo utilizando a biblioteca `pandas`, você pode utilizar o seguinte trecho de código:

```python
import pandas as pd

# Carregando o arquivo CSV
dados_contas = pd.read_csv("/content/contas_saldos.csv")

# Exibindo as primeiras linhas
display(dados_contas.head())
```

## 📈 Análises Práticas Executadas

* **`dados_contas.info()`**: Exibe o tipo de dado de cada coluna e se existem valores ausentes (nulos).
* **`dados_contas.describe()`**: Gera estatísticas descritivas básicas como média dos saldos, desvio padrão, valor mínimo, máximo e quartis.
