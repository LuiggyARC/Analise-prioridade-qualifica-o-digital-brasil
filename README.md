# Análise de Prioridade para Qualificação Digital no Brasil

Projeto de análise de dados para identificar quais Unidades da Federação apresentam maior prioridade para ações de qualificação digital no Brasil.

A análise combina indicadores de mercado de trabalho, renda, acesso digital e dinamismo do emprego formal para construir o **IPQD — Índice de Prioridade para Qualificação Digital**.

## Objetivo

Responder à seguinte pergunta analítica:

> Quais estados brasileiros combinam maior vulnerabilidade no mercado de trabalho com maior necessidade de políticas de qualificação digital?

O projeto foi estruturado como uma análise executiva, com foco em tomada de decisão, visualização em Power BI e apresentação em PowerPoint.

## Ferramentas utilizadas

- Python para tratamento, validação e análise exploratória
- Power BI para construção do dashboard
- PowerPoint para apresentação executiva
- GitHub para documentação e versionamento do projeto
- Bases públicas do IBGE, PNAD Contínua, IPEA e Novo CAGED

## Estrutura do repositório

```text
.
├── apresentacao/
│   └── apresentacao_ipqd_qualificacao_digital.pptx
├── dados/
│   ├── base_ipqd_estados_metodologica.csv
│   ├── base_ipqd_estados_metodologica.xlsx
│   ├── base_ipqd_estados_validada.csv
│   └── base_ipqd_estados_validada.xlsx
├── graficos/
│   ├── grafico_01_top10_ipqd_validado.png
│   ├── grafico_02_ipqd_medio_regiao.png
│   ├── grafico_03_desemprego_vs_internet.png
│   ├── grafico_04_renda_vs_ipqd.png
│   └── grafico_05_composicao_scores_top10.png
├── metodologia/
│   └── metodologia_ipqd.md
└── relatorios/
    ├── insights_etapa2.csv
    └── relatorio_etapa2_analise_exploratoria.md
```

## Índice criado

O principal indicador do projeto é o **IPQD Validado**, construído como índice comparativo entre estados.

Pesos utilizados:

| Dimensão | Peso |
|---|---:|
| Taxa de desocupação | 30% |
| Baixa renda | 30% |
| Baixo acesso digital | 20% |
| Baixo dinamismo do emprego formal | 20% |

A versão validada do índice removeu variáveis com rastreabilidade menos consolidada, como escolaridade e população, mantendo-as apenas como variáveis auxiliares de contexto.

## Principais resultados

Top 5 UFs com maior prioridade pelo IPQD Validado:

| Posição | UF | Região | Leitura |
|---:|---|---|---|
| 1 | Maranhão | Nordeste | Prioridade muito alta |
| 2 | Piauí | Nordeste | Prioridade muito alta |
| 3 | Alagoas | Nordeste | Prioridade muito alta |
| 4 | Amapá | Norte | Prioridade muito alta |
| 5 | Pernambuco | Nordeste | Prioridade alta |

A análise indica concentração de prioridade principalmente nos estados do **Nordeste** e parte do **Norte**, regiões onde se combinam baixa renda, maior vulnerabilidade no mercado de trabalho, barreiras de acesso digital e menor dinamismo formal.

## Visualizações principais

- Ranking das UFs por IPQD Validado
- IPQD médio por região
- Relação entre desemprego e acesso digital
- Relação entre renda e prioridade de qualificação
- Composição dos fatores do índice nos estados prioritários

## Decisão metodológica

Este projeto trata o IPQD como uma ferramenta analítica comparativa, e não como indicador oficial.

Bases públicas podem sofrer revisões, atualizações, recortes metodológicos e pequenas variações entre divulgações oficiais. Isso não invalida a análise quando as fontes, limitações e decisões metodológicas estão documentadas.

O saldo CAGED foi utilizado como medida relativa de dinamismo do mercado formal por UF, não como fechamento contábil oficial do saldo nacional.

A população e a escolaridade foram mantidas como dimensões auxiliares, não compondo o índice principal validado.

## Arquivos principais

- `dados/base_ipqd_estados_metodologica.csv`: base principal recomendada para análise e Power BI
- `apresentacao/apresentacao_ipqd_qualificacao_digital.pptx`: apresentação executiva do projeto
- `metodologia/metodologia_ipqd.md`: documentação da metodologia do índice
- `relatorios/relatorio_etapa2_analise_exploratoria.md`: relatório da análise exploratória

## Como usar

1. Baixe a base metodológica em `dados/`.
2. Importe no Power BI.
3. Use `IPQD_Validado` como indicador principal.
4. Utilize `Ranking_IPQD_Validado`, `Regiao` e `Prioridade_Executiva` como filtros e segmentadores.
5. Consulte a pasta `metodologia/` para justificar as decisões do projeto.

## Conclusão

A qualificação digital não deve ser distribuída de forma genérica. Os dados indicam que ações mais efetivas precisam considerar a combinação entre vulnerabilidade econômica, acesso digital e dinamismo do mercado formal.

O IPQD ajuda a transformar esses fatores em uma visão comparativa, permitindo priorizar estados onde programas de qualificação digital podem gerar maior impacto social e econômico.
