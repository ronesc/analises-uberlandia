# 01 - Os bairros de Uberlândia (Censo 2022)

## Pergunta
Qual é o bairro mais populoso? Onde a cidade está mais apertada? Quais bairros têm mais jovens e quais têm mais idosos?

## Dados
IBGE, Censo Demográfico 2022, agregados por bairros oficiais. São 75 bairros em Uberlândia. O notebook baixa os arquivos direto do FTP do IBGE.

## Como o código funciona, em linhas gerais
1. Baixa três CSVs (básico, demografia, cor ou raça) e a malha geográfica dos bairros.
2. Filtra o código do município (3170206) e confere o total com o número oficial.
3. Junta tudo numa tabela só e calcula densidade e percentuais por faixa etária.
4. Gera ranking dos bairros mais populosos, mapas de população e composição racial, e a pirâmide etária da cidade.

## Principal achado
Santa Mônica é o bairro mais populoso (37.665 pessoas). Pequis tem 40% de moradores com até 19 anos, enquanto Fundinho tem 38,6% com 60 ou mais.

## Detalhe importante
A soma dos bairros (680 mil) é menor que a população total do município (713 mil), porque o arquivo cobre só os bairros oficiais da área urbana. Zona rural fica de fora.
