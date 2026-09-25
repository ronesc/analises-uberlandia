# 05 - As empresas de Uberlândia (CEMPRE, IBGE)

Análise do cadastro de empresas da cidade: quantas são, de quais setores, qual o porte e quando foram fundadas.

## Fonte

CEMPRE (Cadastro Central de Empresas) do IBGE, via API do SIDRA:

- Tabela 9582 (empresas por município, setor CNAE, faixa de pessoal ocupado e ano de fundação): https://sidra.ibge.gov.br/tabela/9582
- Tabela 3421 (unidades locais, pessoal ocupado e salário médio): https://sidra.ibge.gov.br/tabela/3421

Consultas usadas (Uberlândia = código 3170206):

- `https://apisidra.ibge.gov.br/values/t/9582/n6/3170206/v/2585/p/2024/c12762/allxt` (por setor)
- `https://apisidra.ibge.gov.br/values/t/9582/n6/3170206/v/2585/p/2024/c319/allxt` (por porte)
- `https://apisidra.ibge.gov.br/values/t/9582/n6/3170206/v/2585/p/2024/c12386/allxt` (por ano de fundação)
- `https://apisidra.ibge.gov.br/values/t/9582/n6/3170206/v/2585/p/all` (total por ano)
- `https://apisidra.ibge.gov.br/values/t/3421/n6/3170206/v/all/p/last 5` (ocupação e salário)

## Arquivos

- `analise_empresas_uberlandia.ipynb`: notebook com a análise completa
- `dados/cempre_uberlandia.csv`: dados da cidade usados no notebook
- `graficos/`: gráficos gerados

## Como rodar

```
pip install -r ../requirements.txt
jupyter notebook analise_empresas_uberlandia.ipynb
```

## Limitações

O CEMPRE conta empresas e organizações com pelo menos um vínculo empregatício. MEI sem funcionário e autônomos não entram. A tabela 9582 vai até 2024; a 3421 (ocupação e salário) está publicada até 2021.
