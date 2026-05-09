# sales-forecast-ml
Sales for📈 Sales Forecast — Machine Learning + Power BI
Previsão de vendas com Machine Learning em Python e visualização interativa no Power BI.

🎯 Objetivo
Desenvolver um pipeline completo de dados que utiliza modelos de Machine Learning para prever o faturamento futuro de uma empresa, com os resultados apresentados em um dashboard executivo no Power BI.

🖼️ Dashboard Preview

Print ou GIF do dashboard aqui


🗂️ Estrutura do Projeto
📦 sales-forecast-powerbi
├── 📂 data
│   ├── raw/                  # Dados brutos originais
│   └── processed/            # Dados tratados prontos para o modelo
├── 📂 notebooks
│   ├── 01_eda.ipynb          # Análise exploratória dos dados
│   └── 02_model.ipynb        # Treinamento e avaliação do modelo
├── 📂 src
│   ├── etl.py                # Limpeza e transformação dos dados
│   ├── train.py              # Treinamento e exportação do modelo
│   └── predict.py            # Geração das previsões
├── 📂 outputs
│   └── predictions.csv       # Previsões consumidas pelo Power BI
├── 📂 powerbi
│   └── dashboard.pbix        # Dashboard Power BI
├── 📂 images
│   └── dashboard_preview.png
├── requirements.txt
└── README.md

🔄 Fluxo do Projeto
Dados Brutos → ETL (Python) → Modelo ML → predictions.csv → Power BI Dashboard

🛠️ Tecnologias Utilizadas
TecnologiaFinalidadePython 3.11+Linguagem principalPandasManipulação e limpeza de dadosScikit-learnModelo de Machine LearningMatplotlib / SeabornVisualizações exploratóriasJoblibSerialização do modelo treinadoPower BIDashboard interativo

📊 Dataset
Projeto desenvolvido com o Sample Superstore Dataset, um dataset público com dados de vendas de uma empresa americana de varejo.

🔗 Download no Kaggle
~10.000 registros de pedidos entre 2019 e 2022
Colunas principais: Order Date, Sales, Category, Region, Profit


🚀 Como Executar
1. Clone o repositório
bashgit clone https://github.com/seu-usuario/sales-forecast-powerbi.git
cd sales-forecast-powerbi
2. Instale as dependências
bashpip install -r requirements.txt
3. Execute o pipeline
bash# Limpeza e transformação dos dados
python src/etl.py

# Treinamento do modelo
python src/train.py

# Geração das previsões
python src/predict.py
4. Abra o dashboard
Abra o arquivo powerbi/dashboard.pbix no Power BI Desktop e atualize a fonte de dados apontando para outputs/predictions.csv.

📦 Instalação das Dependências
pandas
scikit-learn
matplotlib
seaborn
joblib
