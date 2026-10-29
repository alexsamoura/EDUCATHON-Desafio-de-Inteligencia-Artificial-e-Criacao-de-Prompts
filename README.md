# Ciclistas de São Miguel Paulista: prompt para uma solução com IA

Projeto individual feito no **EDUCATHON 2026**, desafio de engenharia de prompt promovido pelo Instituto Eldorado em parceria com a IBM SkillsBuild (01 a 03/10/2026, 48 horas, online).

**Resultado:** [preencher: classificação ou "participação"]

## O desafio

O enunciado tinha duas partes:

1. Descrever uma necessidade real da sua cidade: o problema, quem é mais afetado e por que resolver importa (até 2.000 caracteres).
2. Escrever um prompt que leve a IA a propor a melhor solução e a apresentá-la para aprovação, com contexto, objetivo, papel da IA e formatação (até 4.000 caracteres).

A banca avaliou o prompt, não a resposta da IA. Critérios e pesos: compreensão do desafio (25), clareza e organização (20), aplicabilidade prática (20), orientação da resposta (15), boas práticas de prompt (10), inovação (10).

## O problema escolhido

Ciclistas que usam a bicicleta como transporte no trajeto entre a estação da CPTM e o centro comercial de São Miguel Paulista, zona leste de São Paulo: trabalhadores, estudantes, entregadores e famílias de baixa renda. Pedalam por trechos sem ciclovia, com buracos e pista escorregadia, dividindo a via com ônibus, carros e motos.

Escolhi esse recorte porque morei na região e usava a bicicleta como transporte.

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| [parte-1-problema.md](parte-1-problema.md) | Texto do problema, como submetido |
| [parte-2-prompt.md](parte-2-prompt.md) | Prompt submetido e a lógica de cada bloco |

## Decisões de prompt

- **Comparar antes de escolher.** O prompt pede 3 alternativas e uma tabela (viabilidade para 5 pessoas, impacto, custo, prazo) antes da recomendação. Sem isso, o modelo tende a entregar a primeira ideia que aparece.
- **Proibir invenção.** A IA não pode inventar dados, ruas ou programas. Qualquer ponto específico não fornecido sai marcado como hipótese.
- **Resultado acionável.** A solução precisa servir de base para pedidos à CET e à Subprefeitura, não ficar só no diagnóstico.
- **Acesso e privacidade.** Se houver coleta de relatos, precisa funcionar por WhatsApp ou áudio e proteger localização conforme a LGPD.
- **Escopo pequeno.** Piloto com indicadores mensuráveis, sem promessa de impacto que não dá para comprovar.

## Revisão de dados (depois da submissão)

Ao revisar as fontes para publicar este repositório, encontrei divergências nos números que usei. Os textos acima ficaram como foram enviados; a correção está aqui.

| Afirmação submetida | O que encontrei | Status |
|---|---|---|
| Viagens de bicicleta cresceram 12% (2017–2023) "na cidade" | A Pesquisa OD cobre a Região Metropolitana, não só a capital. Uma fonte reporta crescimento de 25,2% (377 mil para 472 mil viagens/dia); outra reporta estabilidade em cerca de 400 mil. Não encontrei o número de 12%. | Corrigir: conferir no relatório oficial do Metrô |
| Total de deslocamentos "caiu para 18,5%" / "caiu 18,5%" | Queda de cerca de 15,1% (42 milhões para 35,6 milhões de viagens/dia, RMSP). Na Parte 1 também havia erro de redação ("caiu para"). | Corrigir para cerca de 15% |
| São Miguel com 18,75 km de ciclovias/ciclofaixas contra mais de 30 km em Pinheiros (Agência Mural) | Não localizei a reportagem original. | Pendente: confirmar no GeoSampa |
| Mortes de ciclistas na capital: 34 (2023) para 44 (2024), Infosiga | Não verificado nesta revisão. | Pendente: confirmar no Infosiga SP |

Fontes consultadas na revisão:

- [DComércio: uso de veículo particular na Grande SP supera o de transporte público](https://www.dcomercio.com.br/publicacao/s/uso-de-veiculo-particular-na-grande-sp-supera-o-de-transporte-publico)
- [Technibus: ônibus é o modo de transporte com maior retração depois da pandemia](https://technibus.com.br/2025/02/12/onibus-e-o-modo-de-transporte-com-maior-retracao-depois-da-pandemia)

O erro principal foi usar número de segunda mão sem abrir o relatório da Pesquisa OD. Num trabalho real, o dado errado no contexto do prompt vai direto para a resposta da IA, mesmo com a instrução "não invente dados".

## Fontes de dados citadas no prompt

- Pesquisa Origem e Destino 2023 (Metrô de São Paulo)
- GeoSampa (Prefeitura de São Paulo)
- Infosiga SP (Governo do Estado de São Paulo)
- SP156 (Prefeitura de São Paulo)

## Licença

Texto e prompt sob [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.pt-br). Pelo regulamento do EDUCATHON, a autoria das soluções é dos participantes, e a organização pode usá-las para fins institucionais e educacionais, sem fins comerciais.

**Autora:** Alexsandra Moura
