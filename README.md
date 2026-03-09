
---

<p align="justify"><h1>Análise de Performance e Risco-Retorno</h1></p>

<p align="justify">Este documento apresenta a análise de desempenho de três estratégias de investimento — Risco Baixo, Médio e Alto — processadas através do seu ambiente Python. O foco principal recai sobre a eficiência de cada carteira quando ajustada pela volatilidade do mercado, utilizando o <b>Índice de Sharpe</b> como métrica balizadora para a tomada de decisão.</p>

<p align="justify"><h3>1. Metodologia e Parâmetros</h3></p>

<p align="justify">A análise considera uma Taxa Livre de Risco de 5% ao ano (<b>taxa_livre_risco_anual = 0.05</b>), que serve como o patamar mínimo de rentabilidade esperada sem exposição ao risco variável. Os retornos foram calculados com base em uma estratégia de <b>pesos iguais</b> para cada ativo dentro dos portfólios, garantindo que a diversificação não seja enviesada por uma única ação de grande porte.</p>

<p align="justify"><h3>2. O Conceito: O Índice de Sharpe</h3></p>

<p align="justify">O Índice de Sharpe é uma ferramenta fundamental para medir a qualidade de um investimento. Ele não olha apenas para o retorno final, mas sim para quanto risco foi necessário correr para alcançar esse resultado. Matematicamente, o índice <b>S</b> é calculado pela razão entre o retorno excedente e a volatilidade do portfólio:</p>

<p align="center">
<b>S = (R<sub>p</sub> - R<sub>f</sub>) / σ<sub>p</sub></b>
</p>

<p align="justify">Onde <b>R<sub>p</sub></b> é o retorno do portfólio, <b>R<sub>f</sub></b> é a taxa livre de risco e <b>σ<sub>p</sub></b> representa o desvio padrão (volatilidade). Um índice maior indica uma carteira mais eficiente; se duas carteiras têm o mesmo retorno, a que tiver a menor oscilação apresentará o melhor resultado.</p>

<p align="justify"><h3>3. Resultados e Análise Justificada</h3></p>

<p align="justify">Com base nos dados processados, observamos que a estratégia de <b>Risco Baixo Diversificado</b> obteve o melhor desempenho relativo com um índice de <b>0.61</b>, superando as demais em termos de consistência. Em contrapartida, o portfólio de <b>Risco Alto</b>, apesar de entregar o maior retorno mensal bruto (1.91%), apresentou um Sharpe de <b>0.52</b>, demonstrando que o ganho extra é acompanhado por uma volatilidade proporcionalmente elevada. Por fim, o grupo de <b>Risco Médio Diversificado</b> foi o menos eficiente (0.35), indicando que os ativos selecionados não compensaram o risco assumido frente à taxa de 5% definida no projeto.</p>

---

