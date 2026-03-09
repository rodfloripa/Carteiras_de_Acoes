

---

<p align="justify"><h1>Carteiras de Ações: O Impacto da Selic a 15,00%</h1></p>


<p align="justify">Este relatório detalha a análise de desempenho de portfólios sob um cenário de alta taxa de juros (<b>Selic a 15,00% a.a.</b>), utilizando técnicas avançadas de estatística para mensuração de risco. A principal inovação desta análise é a substituição do desvio padrão convencional pela escala da <b>Distribuição t de Student</b>.</p>

<p align="justify"><h3>1. Metodologia: Volatilidade Robusta via Distribuição t</h3></p>

<p align="justify">Em mercados voláteis, a distribuição normal (Gaussiana) frequentemente falha ao não capturar as "caudas gordas" — eventos extremos que ocorrem com mais frequência do que a teoria clássica prevê.</p>

<p align="justify">Ao utilizarmos a função <code>t.fit()</code> para extrair o parâmetro de <b>escala</b>, a volatilidade calculada torna-se <b>robusta</b>. Isso significa que o Índice de Sharpe agora reflete uma relação risco-retorno que ignora ruídos excessivos e <i>outliers</i>, proporcionando uma visão muito mais fiel da eficiência do capital investido em ativos de alta volatilidade, como PETR4 ou MGLU3.</p>

<p align="justify"><h3>2. Resultados e Análise de Eficiência (Benchmark: Selic 15%)</h3></p>

<p align="justify">Os resultados obtidos demonstram como a barreira dos 15% de taxa livre de risco impacta a atratividade da renda variável:</p>

| Estratégia | Cenário | Retorno Mensal | Sharpe Robusto (t) |
| --- | --- | --- | --- |
| **Risco Baixo** | Original | 1,18% | **-0,07** |
| **Risco Baixo** | **Diversificado** | **1,31%** | **0,06** |
| **Risco Médio** | Original | 1,36% | **0,07** |
| **Risco Médio** | Diversificado | 1,21% | **-0,03** |
| **Risco Alto** | **Original** | **1,91%** | **0,26** |
| **Risco Alto** | Diversificado | 1,87% | **0,25** |

<p align="justify"><h3>3. Conclusão Técnica</h3></p>

<p align="justify">A análise robusta confirma que, com a Selic atual, portfólios de <b>Risco Baixo</b> e <b>Médio</b> muitas vezes não compensam o risco de mercado, apresentando Sharpe negativo ou próximo de zero. A estratégia de <b>Risco Alto</b>, no entanto, destaca-se com um Sharpe de <b>0,26</b>, indicando que a volatilidade extra — agora medida de forma precisa pela Distribuição t — é devidamente recompensada com um prêmio de risco real acima da renda fixa.</p>

---

