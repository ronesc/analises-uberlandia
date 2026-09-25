# 02 - De onde vem o dinheiro de Uberlândia

## Pergunta
Quanto a prefeitura arrecada por ano e de onde vem esse dinheiro?

## Dados
API pública do SICONFI (Tesouro Nacional), RREO dos anos de 2019 a 2024. O notebook chama a API direto, sem download manual.

## Como o código funciona, em linhas gerais
1. Chama a API do Tesouro para cada ano, pegando a receita realizada (Anexo 01 do RREO).
2. Monta a série anual do total arrecadado.
3. Separa os grandes grupos da receita corrente e compara receita própria com transferências.
4. Fecha com o número de conversa: quanto entra por dia no caixa.

## Principal achado
R$ 4,2 bilhões em 2024, ou R$ 11,5 milhões por dia. Metade (51%) da receita corrente vem de transferências da União e do Estado; impostos próprios respondem por 28%.

## Detalhe importante
Valores nominais, sem correção pela inflação. O detalhe por imposto (IPTU, ISS) não está no SICONFI, fica para uma análise futura.
