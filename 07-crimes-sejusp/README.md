# 07 - Crimes violentos em Uberlândia (2019 a 2025)

Análise dos registros de crimes violentos da cidade: total por ano, tipos de crime, série de homicídios com taxa por 100 mil habitantes e o comportamento mês a mês em 2024 e 2025.

## O que o notebook mostra

- total de crimes violentos por ano (2019 a 2025)
- participação de cada tipo de crime (roubo, homicídio, estupro, extorsão, sequestro, feminicídio)
- série de homicídios com taxa por 100 mil habitantes
- tendência mensal de 2024 e 2025

## De onde vêm os dados

Banco de Crimes Violentos da SEJUSP-MG, no portal de dados abertos de Minas Gerais:
https://dados.mg.gov.br/dataset/crimes-violentos

Baixei os CSVs anuais (2019 a 2025) e filtrei as linhas de Uberlândia (código IBGE 317020). O resultado está em `dados/crimes_violentos_uberlandia_2019_2025.csv`, então o notebook roda direto.

## Ressalvas

- a base cobre só os crimes violentos da SEJUSP; furto e tráfico estão em outras bases do portal
- são registros de ocorrência policial; crimes com subnotificação (como estupro) aparecem menores do que a realidade

## Como rodar

```
pip install -r ../requirements.txt
jupyter notebook analise_crimes_uberlandia.ipynb
```
