
---

<p align="justify"><h1>Carteiras de Ações: O Impacto da Selic a 15,00%</h1></p>

<p align="justify">Este relatório detalha a análise de desempenho de portfólios escolhidos de 20 ações sob um cenário de alta taxa de juros (<b>Selic a 15,00% a.a.</b>), utilizando técnicas avançadas de estatística para mensuração de risco. A principal inovação desta análise é a substituição do desvio padrão convencional pela escala da <b>Distribuição t de Student</b>.</p>

<p align="justify"><h3>1. Metodologia: Volatilidade Robusta via Distribuição t</h3></p>

<p align="justify">Em mercados voláteis, a distribuição normal (Gaussiana) frequentemente falha ao não capturar as "caudas gordas" — eventos extremos que ocorrem com mais frequência do que a teoria clássica prevê.</p>

<p align="justify">Ao utilizarmos a função <code>t.fit()</code> para extrair o parâmetro de <b>escala</b>, a volatilidade calculada torna-se <b>robusta</b>. Isso significa que o risco mensurado ignora ruídos excessivos e <i>outliers</i>, proporcionando uma visão muito mais fiel da eficiência do capital investido em ativos de alta volatilidade.</p>

<p align="justify"><h3>2. O Índice de Sharpe Adaptado</h3></p>

<p align="justify">O Índice de Sharpe tradicional foi recalibrado para este estudo com dois ajustes críticos:</p>

* **Benchmark Elevado:** Consideramos a Selic de **15,00% a.a.** como o custo de oportunidade. Isso significa que qualquer retorno abaixo de aproximadamente 1,17% ao mês resulta em um Sharpe negativo, indicando que o investimento não superou a renda fixa.
* **Denominador de Escala:** Em vez do desvio padrão comum, utilizamos a escala da Distribuição t, o que permite uma avaliação mais justa de portfólios com ativos voláteis que apresentam saltos bruscos de preço.

<p align="justify"><h3>3. Resultados e Análise de Eficiência</h3></p>

| Estratégia | Cenário | Retorno Mensal | Sharpe Robusto (t) |
| --- | --- | --- | --- |
| **Risco Baixo** | Original | 1,18% | **-0,07** |
| **Risco Baixo** | **Diversificado** | **1,31%** | **0,06** |
| **Risco Médio** | Original | 1,36% | **0,07** |
| **Risco Médio** | Diversificado | 1,21% | **-0,03** |
| **Risco Alto** | **Original** | **1,91%** | **0,26** |
| **Risco Alto** | Diversificado | 1,87% | **0,25** |

<p align="justify"><h3>4. Conclusão Técnica</h3></p>

<p align="justify">A análise confirma que, com a Selic a 15%, a maioria das estratégias de <b>Risco Baixo</b> e <b>Médio</b> apresenta dificuldade em gerar prêmio de risco positivo, com índices de Sharpe próximos de zero ou negativos.</p>

<p align="justify">O destaque absoluto é a estratégia de <b>Risco Alto (Original)</b>, que atingiu um Sharpe de <b>0,26</b>. Este resultado demonstra que, ao medir a volatilidade de forma robusta pela Distribuição t, o retorno excedente desses ativos justifica a exposição ao risco mesmo em um ambiente de juros extremamente elevados.</p>

---
