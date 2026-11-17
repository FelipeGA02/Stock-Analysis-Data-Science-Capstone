# Análise de carteira de ações e de chamadas de emergência (911)

Dois projetos de ciência de dados em Jupyter Notebook: análise de risco e retorno de uma carteira de ações com dados do Yahoo Finance e análise exploratória de chamadas de emergência 911 do condado de Montgomery (Pensilvânia, EUA).

## Problema que resolve e para quem

- **Carteira de ações:** quem investe ou analisa investimentos precisa comparar ativos por retorno, volatilidade e retorno ajustado ao risco, e entender como a diversificação muda o resultado da carteira.
- **Chamadas 911:** gestores de serviços de emergência precisam saber quais tipos de ocorrência são mais comuns e em que dias, meses e horários a demanda se concentra, para dimensionar equipes.

Os notebooks foram desenvolvidos como atividade acadêmica (projeto *capstone*) e servem como exemplos práticos de análise exploratória, visualização e finanças quantitativas com Python.

## Tecnologias utilizadas

Python, Pandas, NumPy, Matplotlib, Seaborn, yfinance, SciPy (otimização da fronteira eficiente) e Jupyter Notebook.

## Projetos

### 1. Análise de carteira de ações — `Stock-Analysis-Capstone-Project .ipynb`

- Download de preços históricos com yfinance (ações como AAPL, JNJ, KO, TSLA e XOM, de 2018 a 2023).
- Retornos diários e acumulados, histogramas de retornos e simulação de um investimento inicial.
- Índice de Sharpe anualizado por ação.
- Volume negociado e volume financeiro diário.
- Análise técnica: média móvel de 60 dias e Bandas de Bollinger.
- Retornos ponderados da carteira e fronteira eficiente de Markowitz (minimização da volatilidade para cada retorno-alvo).

### 2. Chamadas de emergência 911 — `DataCapstone_Project.ipynb`

- Base pública do Kaggle com chamadas 911 do condado de Montgomery (PA), com latitude, longitude, CEP, município, título e data/hora.
- Criação de atributos: motivo da chamada (EMS, Fire, Traffic) a partir do título; hora, mês e dia da semana a partir da data.
- CEPs e municípios com mais chamadas, contagem por motivo, por dia da semana e por mês, tendência mensal com regressão linear (`lmplot`), mapas de calor e *clustermaps* de dia da semana x hora e dia da semana x mês.
- Parte 2: análise exploratória de uma base de desempenho de estudantes (`students.csv`) com estatísticas descritivas, histogramas, *box plots*, dispersão e correlações.

## Como executar

Pré-requisitos: Python 3 e Jupyter Notebook (ou Anaconda).

```bash
git clone https://github.com/FelipeGA02/Stock-Analysis-Data-Science-Capstone.git
cd Stock-Analysis-Data-Science-Capstone
pip install pandas numpy matplotlib seaborn yfinance scipy jupyter
jupyter notebook
```

- O notebook de ações baixa os dados direto do Yahoo Finance (precisa de internet).
- As bases do notebook 911 não estão no repositório: baixe o `911.csv` (dataset "Emergency - 911 Calls", Montgomery County, no Kaggle) e um `students.csv` de desempenho de estudantes, e salve ambos na mesma pasta do notebook.

## Minha contribuição

Projeto individual: código, modelagem e documentação de minha autoria.

## Demonstração

Os gráficos (preços ajustados, histogramas de retornos, médias móveis, Bandas de Bollinger, fronteira eficiente, contagens por motivo e mapas de calor) ficam salvos nas saídas dos próprios notebooks e podem ser vistos diretamente no GitHub, abrindo cada arquivo `.ipynb`.

## Resultados

- **Ações:** o notebook compara risco e retorno dos ativos pelo índice de Sharpe e mostra, na fronteira eficiente, como a combinação de ativos muda a volatilidade da carteira para cada retorno esperado.
- **911:** as chamadas de emergência médica (EMS) são o motivo mais frequente, e as ocorrências de trânsito se concentram em horários comerciais.
