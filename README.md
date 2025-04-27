# Projeto de ETL: Análise de Vendas de Video Games 🎮

## Descrição
Este projeto faz parte da disciplina de Ciência de Dados da pós-graduação e tem como objetivo aplicar os conceitos de **ETL (Extract, Transform, Load)** na prática.  
O foco está em extrair dados de vendas de video games, realizar a limpeza e transformação dos dados, e preparar o conjunto para futuras análises.

O dataset utilizado foi retirado do [Kaggle - Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogamesales).

---

## Etapas do ETL

### 1. Extração (Extract)
- Carregamento do dataset `vgsales.csv` utilizando `pandas`.
- Primeira inspeção dos dados (`head`, `info`, identificação de valores nulos e duplicados).

### 2. Transformação (Transform)
- Tratamento de valores faltantes:
  - Preenchimento de valores nulos na coluna `Year`.
  - Análise e preenchimento de valores na coluna `Publisher`.
- Verificação e limpeza de caracteres não numéricos ou inconsistentes em colunas textuais (`Name`, `Genre`, `Publisher`).
- Preparação inicial para padronização das variáveis categóricas.

### 3. Carga (Load)
- Neste momento, a carga está sendo preparada para as próximas etapas, como a exportação para um arquivo `.csv` ou a integração com um banco de dados (não implementado ainda nesta fase inicial).

---

## Tecnologias Utilizadas

- Python 3.11+
- Bibliotecas:
  - `pandas` (manipulação de dados)
  - `matplotlib` e `seaborn` (para geração de gráficos exploratórios - em etapas futuras)

---

## Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repo-etl-videogames.git


## Contato
- Feito por Matheus Rosetti Lopes
- Entre em contato por matheus.rosetti@outlook.com
