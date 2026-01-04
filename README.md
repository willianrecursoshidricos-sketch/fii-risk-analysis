# fii-risk-analysis
Análise de risco de Fundos Imobiliários brasileiros usando Web Scraping, regras técnicas e Power BI
# 📊 Análise de Risco de Fundos Imobiliários Brasileiros

Este projeto tem como objetivo analisar Fundos Imobiliários (FIIs) negociados no Brasil,
criando **alertas de risco de dividendos e setor**, além de um **score técnico**, utilizando:

- Web Scraping
- Análise de dados em Python
- Regras técnicas (risk scoring)
- Visualização em Power BI

---

## 🔍 Etapas do Projeto

### 1️⃣ Coleta de Dados (Web Scraping)

Os dados utilizados neste projeto foram obtidos a partir de informações
publicamente disponíveis no site **Funds Explorer**  
(https://www.fundsexplorer.com.br).

A coleta foi realizada por meio de técnicas de Web Scraping, com o objetivo
exclusivo de **análise educacional e exploratória**, respeitando o caráter
informativo dos dados disponibilizados pela plataforma.

Os dados coletados incluem:
- Fundos Imobiliários (tickers)
- Setor de atuação
- Dividend Yield
- Liquidez diária
- Indicadores de mercado (ex: P/VP)


### 2️⃣ Engenharia de Variáveis
- Normalização dos dados
- Criação de indicadores técnicos
- Construção do `SCORE_TECNICO`

### 3️⃣ Alertas de Risco
- `ALERTA_DIVIDENDO`: risco de queda de dividendos
- `ALERTA_SETOR`: risco estrutural do setor do FII

### 4️⃣ Dashboard Interativo (Power BI)
- Visualização clara e didática
- Foco em usuários leigos
- Indicadores visuais de risco (cores e ícones)

---

## 📈 Exemplos do Dashboard

### 🔴🟡🟢 Alertas de Risco
![Alertas](powerbi/dashboard_overview.png)

### 📊 Análise por Setor
![Setor](powerbi/alerta_setor.png)

---

## 🛠️ Tecnologias Utilizadas
- Python (Pandas, NumPy)
- Web Scraping
- Power BI
- Jupyter Notebook

---

## ⚠️ Aviso
Este projeto tem fins educacionais e analíticos.
Não constitui recomendação de investimento.
