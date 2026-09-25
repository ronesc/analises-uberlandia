# 03 - O mercado de trabalho formal em Uberlândia (CAGED 2025)

Análise das admissões e desligamentos de empregos com carteira assinada em Uberlândia durante 2025, mês a mês, por setor, por salário e por escolaridade.

## O que o notebook mostra

- saldo de vagas formais mês a mês (admissões menos desligamentos)
- quais setores criaram e quais fecharam vagas no ano
- mediana salarial das contratações por setor
- escolaridade de quem foi contratado

## De onde vêm os dados

Microdados do Novo CAGED (Ministério do Trabalho e Emprego), arquivos mensais de 2025:
ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED/2025/

Cada arquivo mensal tem o Brasil inteiro (mais de 400 MB descompactado). Baixei os 12 meses e filtrei só as linhas de Uberlândia. O resultado já está em `dados/uberlandia_caged_2025.csv`, então o notebook roda direto sem baixar nada.

## Ressalvas

- o CAGED cobre só emprego formal; trabalho informal e autônomo ficam de fora
- o dado é de movimentação (quem entrou e saiu), não de estoque de empregados
- o salário é o valor declarado na contratação

## Como rodar

```
pip install -r ../requirements.txt
jupyter notebook analise_empregos_caged_uberlandia.ipynb
```
