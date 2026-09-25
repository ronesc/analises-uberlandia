# 04 - A frota de Uberlândia (RENAVAM jul/2026)

Análise dos veículos registrados na cidade: tamanho da frota, veículos por habitante, idade média, marcas e modelos mais comuns.

## O que o notebook mostra

- total de veículos e veículos por habitante (cruzando com o Censo 2022)
- distribuição da frota por ano de fabricação
- top 10 marcas e top 12 modelos
- o peso das motos (famílias CG e Biz da Honda) na frota da cidade

## De onde vêm os dados

Dados abertos do RENAVAM (Ministério dos Transportes), arquivo mensal de julho de 2026:
https://dados.transportes.gov.br (conjunto "Registro Nacional de Veículos Automotores - RENAVAM")

O arquivo original tem o Brasil inteiro (cerca de 136 MB compactado). Baixei e filtrei só Uberlândia. O resultado está em `dados/frota_uberlandia_202607.csv`, então o notebook roda direto.

## Ressalvas

- o arquivo não traz um campo de tipo de veículo; a leitura moto x carro é indireta, pelos modelos
- a contagem é de registros ativos no município na competência jul/2026

## Como rodar

```
pip install -r ../requirements.txt
jupyter notebook analise_frota_uberlandia.ipynb
```
