(English version at the end)
# Projeto de ETL: Análise de Vendas de Video Games 

## Descrição

Este projeto faz parte da disciplina de Ciência de Dados da pós-graduação e tem como objetivo aplicar na prática os conceitos de ETL (Extract, Transform, Load). O foco está em extrair dados de vendas de video games, realizar a limpeza e transformação dos dados e armazenar o resultado em um banco de dados relacional para futuras análises.

O dataset original foi obtido do Kaggle: [Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogame-sales-with-ratings).

---

## 📊 Etapas do ETL

### 1. Extração (Extract)
- Leitura do dataset `vgsales.csv` com `pandas`.
- Análise inicial: visualização (`head`), tipos de dados (`info`), valores nulos e duplicados.

### 2. Transformação (Transform)
- Remoção de valores duplicados.
- Preenchimento de valores nulos:
  - `Publisher`: preenchido com a moda da coluna.
  - `Year`: preenchido com a mediana e convertido para `int`.
- Normalização e inspeção de colunas categóricas (`Genre`, `Publisher`).
- Visualização de outliers em colunas numéricas com `seaborn` e `matplotlib`.

### 3. Carga (Load)
- Criação do schema `vgs_etl` no MySQL.
- Criação da tabela `video_game_sales`.
- Exportação do DataFrame para MySQL usando `SQLAlchemy` e `pymysql`.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3.11+
- **Bibliotecas:**
  - `pandas` – Manipulação de dados
  - `matplotlib`, `seaborn` – Análise e visualização de dados
  - `sqlalchemy`, `pymysql` – Integração com MySQL
- **Banco de dados:** MySQL 8+

---

## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repo-etl-videogames.git
   cd seu-repo-etl-videogames

## Contato
- Feito por Matheus Rosetti Lopes
- Entre em contato por matheus.rosetti@outlook.com

-------------------------------------------------------------

# ETL Project: Video Game Sales Analysis 🎮

## Description

This project is part of the Data Science course in the postgraduate program and aims to apply ETL (Extract, Transform, Load) processes in practice. The focus is on extracting, cleaning, transforming, and loading video game sales data into a MySQL database for future analysis.

The dataset was sourced from Kaggle: [Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogame-sales-with-ratings).

---

## 📊 ETL Stages

### 1. Extract
- Dataset loaded from `vgsales.csv` using `pandas`.
- Initial data exploration (head, info, null/duplicate detection).

### 2. Transform
- Removal of duplicate entries.
- Handling missing data:
  - `Publisher`: filled with mode.
  - `Year`: filled with median and converted to integer.
- Categorical normalization of `Genre` and `Publisher`.
- Outlier detection via `seaborn` and `matplotlib`.

### 3. Load
- Schema `vgs_etl` created in MySQL.
- Table `video_game_sales` created and populated using `SQLAlchemy`.

---

## 🛠️ Technologies

- **Language:** Python 3.11+
- **Libraries:**
  - `pandas`
  - `matplotlib`, `seaborn`
  - `sqlalchemy`, `pymysql`
- **Database:** MySQL 8+

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-user/your-etl-videogames-repo.git
   cd your-etl-videogames-repo

