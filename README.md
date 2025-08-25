# 🎬 Dashflix - Análise de Dados do Catálogo da Netflix

Este projeto realiza um processo completo de **ETL (Extração, Transformação e Carga)** e visualização de dados utilizando um **dataset público do catálogo da Netflix** disponibilizado no Kaggle:  

👉 [Netflix Shows Dataset - Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)  

O objetivo é limpar e preparar os dados para análise e, em seguida, criar um **dashboard interativo** para explorar insights sobre o conteúdo disponível na plataforma.

---

## ▶️ Demonstração do Dashboard

Você pode assistir a demonstração do dashboard no LinkedIn através do link abaixo:

👉 [Ver vídeo do Dashflix no LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7365129372015484929/)

---

## ▶️ Executar o ETL no Google Colab

Abra e execute o notebook do ETL diretamente no Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1v-GluTyPtLK1v9LtnFfOLYgXY8nXEcWW?usp=sharing)

> Obs: Para execução completa, faça upload do arquivo `Netflix Dataset.csv` na área de arquivos do Colab.

---

## 📊 Visão Geral do Projeto

O projeto é dividido em duas etapas principais:

### 🔹 Processamento e Limpeza de Dados (ETL)

- Os dados brutos são lidos a partir do arquivo `Netflix Dataset.csv`.  
- Utilizando **Python** e **Pandas**, os dados são limpos e duplicatas removidas.  
- O pipeline de dados é estruturado em camadas (**Bronze, Prata e Ouro**) e armazenado em um banco **SQLite** (simulando um lakehouse).  
- O resultado final desta etapa é o arquivo `netflix_gold.csv` limpo e pronto para análise.

### 🔹 Visualização de Dados em Power BI

- O arquivo `netflix_gold.csv` é utilizado como fonte de dados para criar o dashboard **"Dashflix"** no **Power BI**.  
- O dashboard permite explorar várias métricas:
  - Contagem de filmes vs. séries  
  - Distribuição de conteúdo por país  
  - Classificações etárias mais comuns  
  - Tendências ao longo dos anos  

---

## 🛠️ Tecnologias Utilizadas

- **Python** → Linguagem principal para ETL  
- **Pandas** → Manipulação e análise de dados  
- **SQLAlchemy & SQLite** → Banco de dados local  
- **Power BI** → Criação do dashboard interativo  
- **Google Colab** → Execução do notebook Python  

---

## 📂 Estrutura do Projeto

- `Netflix Dataset.csv` → Dados brutos do catálogo da Netflix (Kaggle)  
- `Netflix_Dataset.ipynb` → Notebook Google Colab com código Python para ETL  
- `netflix_dataset.py` → Script Python gerado a partir do notebook  
- `netflix_gold.csv` → Arquivo final limpo após o ETL  
- `Dashflix.pbix` → Dashboard interativo no Power BI
 
