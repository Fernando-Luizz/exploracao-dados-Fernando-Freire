# Exploração de Dados — ProUni 2020 (MEC)

Este repositório contém uma exploração estatística (EDA) do dataset **ProUni — Bolsas concedidas e perfil dos beneficiários (2020)**, disponível no portal de dados abertos do governo federal.

## Fonte dos dados
- Portal: dados.gov.br  
- Dataset (catálogo): https://dados.gov.br/dados/conjuntos-dados/mec-prouni  
- Órgão responsável: Ministério da Educação (MEC)  
- Formato utilizado: CSV

## O que foi feito no notebook
No arquivo `.ipynb`, foram realizadas as etapas abaixo:
1. **Carregamento do dataset** e verificação do tamanho (nº de linhas e colunas) e das colunas disponíveis.
2. **Preparação/limpeza**: conversão de datas, criação da variável **IDADE** (derivada) e tratamento de possíveis valores inválidos/placeholder (ex.: 31/12/1969).
3. **Valores ausentes e tipos de dados**: análise de `dtype`, contagem e percentual de nulos.
4. **Estatística descritiva (IDADE)**: média, mediana, moda, mínimo, máximo, desvio padrão, variância, quartis e IQR, além de identificação de outliers (regra do IQR).
5. **Análise de variáveis categóricas**: tabelas de frequência (ex.: tipo de bolsa, modalidade, sexo, raça/cor, região e UF).
6. **Visualizações**: histograma de idade, boxplot (idade por tipo de bolsa), gráfico de dispersão (idade vs nº de registros/bolsas por beneficiário) e gráfico de barras por região.

## Principais insights
- A maior parte dos beneficiários está concentrada em **faixas etárias jovens**, com **cauda** para idades mais altas.
- Existem **outliers** de idade (casos bem acima do padrão da maioria).
- Há **concentração geográfica** por região/UF em números absolutos.
- Foi identificada a presença de data **placeholder** (31/12/1969), tratada como ausente para não distorcer a análise.
# exploracao-dados-Fernando-Freire
