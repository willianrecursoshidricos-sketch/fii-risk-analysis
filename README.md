# 📊 fii-risk-analysis
Análise de risco de Fundos Imobiliários brasileiros com Web Scraping, - Machine Learning não supervisionado (Isolation Forest)
 e Power BI

O algoritmo Isolation Forest foi utilizado para identificar comportamentos atípicos
em variáveis como Dividend Yield, liquidez e indicadores técnicos, auxiliando na
criação de alertas de risco de forma objetiva e exploratória.

---

## 📌 Sobre o Projeto

Este projeto tem como objetivo analisar Fundos Imobiliários (FIIs) negociados no Brasil,
utilizando dados públicos para criar **alertas de risco relacionados a dividendos e setores de atuação**.

A proposta não é prever preços ou recomendar investimentos, mas sim **organizar informações
e destacar comportamentos atípicos**, auxiliando análises exploratórias de forma visual e objetiva.

O projeto combina:
- Coleta automatizada de dados
- Análise estatística e técnica
- Machine Learning não supervisionado
- Visualização interativa em Power BI

---

## 🔍 Etapas do Projeto

### 1️⃣ Coleta de Dados (Web Scraping)

Os dados utilizados foram obtidos a partir de informações **publicamente disponíveis**
no site **Funds Explorer**:

https://www.fundsexplorer.com.br

A coleta foi realizada por meio de técnicas de Web Scraping, com finalidade **educacional
e exploratória**, respeitando o caráter informativo da plataforma.

Principais dados coletados:
- Ticker dos Fundos Imobiliários  
- Setor de atuação  
- Dividend Yield  
- Liquidez diária  
- Indicadores de mercado (ex.: P/VP)

---

### 2️⃣ Tratamento dos Dados e Engenharia de Variáveis

Após a coleta, os dados passaram por etapas de preparação, incluindo:

- Limpeza e padronização das variáveis  
- Tratamento de valores ausentes  
- Normalização de indicadores numéricos  
- Construção de métricas auxiliares  
- Criação de um **score técnico (`SCORE_TECNICO`)**

Essas etapas permitem transformar dados brutos em informações comparáveis
entre diferentes fundos.

---

### 3️⃣ Machine Learning – Detecção de Comportamentos Atípicos

Foi aplicada uma abordagem de **Machine Learning não supervisionado** utilizando
o algoritmo **Isolation Forest**.

O modelo é utilizado para:
- Identificar FIIs com comportamento fora do padrão
- Detectar possíveis anomalias nos indicadores analisados
- Apoiar a classificação de risco de forma estatística

O modelo não realiza previsões de preço nem recomendações de investimento,
sendo utilizado apenas como **ferramenta auxiliar de análise**.

---

### 4️⃣ Geração de Alertas de Risco

Com base nos indicadores técnicos e nos resultados do modelo, foram criadas
classificações categóricas de risco:

- **ALERTA_DIVIDENDO**  
  Indica possíveis riscos relacionados à consistência e estabilidade dos dividendos.

- **ALERTA_SETOR**  
  Reflete riscos estruturais associados ao setor de atuação do fundo.

Os alertas são classificados como:
- 🟢 Baixo Risco  
- 🟡 Risco Moderado  
- 🔴 Alto Risco  

---

### 5️⃣ Dashboard Interativo (Power BI)

Os resultados finais foram organizados em um **dashboard interativo no Power BI**,
com foco em clareza visual e usabilidade.

Principais características:
- Interface simples e intuitiva  
- Uso de cores e ícones para indicar níveis de risco  
- Filtros por setor e por fundo  
- Voltado para usuários leigos ou iniciantes em análise financeira  

---

## 📈 Exemplos do Dashboard (Power BI)

### 🔍 Visão Geral dos Fundos
![Imagem](powerbi/powerbidashboard_setor.png)

Tabela com análise individual dos Fundos Imobiliários, exibindo indicadores técnicos,
Dividend Yield e alertas de risco de forma visual e objetiva.

---

### 🏢 Análise de Risco por Setor
![Visão Geral](powerbi/powerbi_dashboard_geral.png)

Análise setorial com detalhamento dos fundos pertencentes a cada categoria,
permitindo identificar concentrações de risco estrutural.

---

## 🛠️ Tecnologias Utilizadas

- Python  
  - Pandas  
  - NumPy  
  - Scikit-learn (Isolation Forest)  
- Web Scraping  
- Jupyter Notebook  
- Power BI  

---

## ⚠️ Aviso Importante

Este projeto não constitui recomendação de investimento.

Os resultados apresentados têm caráter **educacional e exploratório**, servindo
apenas como apoio à análise de dados e estudo do mercado de Fundos Imobiliários.

Este projeto tem fins educacionais e analíticos.
Não constitui recomendação de investimento.
