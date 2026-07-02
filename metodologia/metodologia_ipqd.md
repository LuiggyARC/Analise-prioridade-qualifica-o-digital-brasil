# Metodologia do IPQD — Índice de Prioridade para Qualificação Digital

## 1. Objetivo metodológico

O IPQD foi criado para comparar as Unidades da Federação brasileiras quanto à prioridade relativa para ações de qualificação digital.

O índice não tem pretensão de substituir indicadores oficiais. Ele é uma ferramenta analítica de apoio à decisão, construída para consolidar dimensões de vulnerabilidade econômica, acesso digital e dinamismo do mercado formal.

## 2. Pergunta orientadora

> Quais estados brasileiros combinam maior vulnerabilidade no mercado de trabalho com maior necessidade de ações de qualificação digital?

## 3. Unidade de análise

A unidade de análise utilizada é a Unidade da Federação (UF).

A base metodológica contém 27 UFs, contemplando os 26 estados brasileiros e o Distrito Federal.

## 4. Variáveis utilizadas no índice validado

O IPQD Validado utiliza quatro dimensões principais:

| Dimensão | Variável | Interpretação | Peso |
|---|---|---|---:|
| Mercado de trabalho | Taxa de desocupação | Quanto maior o desemprego, maior a prioridade | 30% |
| Renda | Rendimento médio real | Quanto menor a renda, maior a prioridade | 30% |
| Acesso digital | Percentual de internet | Quanto menor o acesso, maior a prioridade | 20% |
| Dinamismo formal | Saldo CAGED / Estoque CAGED | Quanto menor o dinamismo formal, maior a prioridade | 20% |

## 5. Variáveis auxiliares

As seguintes variáveis foram mantidas como apoio analítico, mas não compõem o IPQD Validado:

| Variável | Uso no projeto |
|---|---|
| População | Escala demográfica e contextualização |
| Escolaridade / Ensino Médio | Contexto de prontidão educacional |
| IPQD original | Versão histórica/expandida do índice |

A decisão de retirar população e escolaridade do índice principal foi tomada para aumentar a rastreabilidade metodológica e reduzir questionamentos sobre fontes auxiliares ainda sujeitas à validação documental por UF.

## 6. Normalização

As variáveis foram transformadas em pontuações comparáveis entre 0 e 100.

A lógica geral foi:

- Indicadores em que valores maiores representam maior vulnerabilidade receberam pontuação maior.
- Indicadores em que valores menores representam maior vulnerabilidade foram invertidos.
- O índice final foi calculado por média ponderada das dimensões.

## 7. Fórmula conceitual

```text
IPQD_Validado =
  30% * Score_Desemprego
+ 30% * Score_Baixa_Renda
+ 20% * Score_Baixo_Acesso_Digital
+ 20% * Score_Baixo_Dinamismo_Formal
```

## 8. Leitura do indicador

Quanto maior o IPQD Validado, maior a prioridade relativa da UF para ações de qualificação digital.

| Faixa interpretativa | Leitura |
|---|---|
| Alta | Prioridade imediata |
| Média | Atenção estratégica |
| Baixa | Baixa urgência relativa |

## 9. Decisão sobre o CAGED

Durante a validação, observou-se diferença entre a soma estadual do saldo CAGED e o total nacional consolidado.

Por esse motivo, o saldo CAGED foi mantido como variável de comparação relativa entre UFs, e não como fechamento contábil oficial do saldo nacional.

Essa decisão é adequada porque o objetivo do projeto não é auditar o CAGED, mas utilizar o dado como uma aproximação do dinamismo formal do mercado de trabalho nos estados.

## 10. Limitações metodológicas

Bases públicas podem sofrer revisões, atualizações, recortes metodológicos e pequenas variações entre divulgações oficiais.

Essas variações não invalidam a análise quando:

- as fontes são documentadas;
- as decisões metodológicas são explicitadas;
- o índice é apresentado como ferramenta comparativa, e não como indicador oficial;
- variáveis com menor rastreabilidade são tratadas como auxiliares.

## 11. Fontes de referência

As bases utilizadas no projeto foram organizadas a partir de dados públicos e referências de:

- IBGE
- PNAD Contínua
- IPEA
- Novo CAGED / Ministério do Trabalho e Emprego

## 12. Uso recomendado

O IPQD Validado deve ser usado para:

- comparar UFs;
- identificar padrões regionais;
- orientar priorização de ações;
- apoiar narrativa executiva em dashboard e apresentação.

Ele não deve ser usado como:

- indicador oficial;
- fechamento estatístico nacional;
- substituto das divulgações originais dos órgãos públicos.
