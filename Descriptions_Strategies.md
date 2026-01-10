## Directional

### 1. [Buy and Hold](1.Directional/1.Buy&Hold.ipynb)
Estratégia direcional básica que mantém posição comprada continuamente no ativo.
Introduz o conceito de preço ajustado e métricas base.

### 2. [Buy and Hold with Risk Scaling](1.Directional/2.Buy&Hol_Risk_Scaling.ipynb)
Extensão do buy and hold com ajuste do tamanho da posição.
Estabiliza o risk utilizando um target em % do capital.

### 3. [Buy and Hold with Variable Risk Scaling](1.Directional/3.Buy&Hold_Variable_Risk_Scaling.ipynb)
Modelo de buy and hold com risco ajustado dinamicamente conforme regimes de volatilidade.
Melhora o Risk Scaling fazendo um ajuste de posição conforme volatilidade histórica do ativo.

### 4. [Buy and Hold Portfolio with Variable Risk](1.Directional/4.Buy&Hold_Portifolio_Variable_Risk.ipynb)
Aplicação do buy and hold com risk scaling em no portfolio "JUMBO".

### 5. [Trend Filter Long](1.Directional/5.Trend_Filter_Long.ipynb)
Estratégia long-only que utiliza um filtro de tendência.
Opera Long quando o ativo esta acima da(s) média(s) de x dias.


### 6. [Trend Filter Long and Short](1.Directional/6.Trend_Filter_Long&Short.ipynb)
Filtro de tendência aplicado para posições compradas e vendidas.
Opera Long quando o ativo esta acima da(s) média(s) de x dias e Short quando está abaixo.

### 7. [Slow Trend Strength Filter](1.Directional/7.Slow_Trend_Strength_Filter.ipynb)
Filtro de força de tendência.
Aprimora o filtro de tendência usando, aplicando um forecast "fast_ma - slow_ma" e ajustando a posição usando a diferênça das médias e volatilidade do preço, diminuindo a posição quando o a média lenta esta maior que a média rápida.

### 8. [Fast Trend Strength Filter](1.Directional/8.Fast_Trend_Strength_Filter.ipynb)
Filtro de força de tendência.
Mesma idéia da estratégia 7, porém a estartégia lenta é "mais rapida" (Prazo curto, de 64 períodos para 16).

### 9. [Multiple Trend Strength Filter](1.Directional/9.Multiple_Trend_Strength_Filter.ipynb)
Combinação de múltiplos filtros de força de tendência em diferentes horizontes.
Combina varias médias móveis para filtrar a posição, utilizando uma média das médias.

### 10. [Basic Carry](1.Directional/10.Basic_Carry.ipynb)
Estratégia baseada em carry.
Estratégia classica de carry trade entre contratos, aumenta/ diminui a posição atual se o próximo contrato do ativo está com carry positivo / negativo.

### 11. [Basic Carry and Trend](1.Directional/11.Basic_Carry&Trend.ipynb)
Combina o filtro das médias com o aumento / diminuição da posição baseada no carry.

---

## Trend Following and Carry

### 12. [Adjusted Trend](2.Trend_Following_and_Carry/12.Adjusted_trend.ipynb)
Modelo de tendência com ajuste de vol.
Faz um filtro de média móvel, mas ajusta a média móvel dividindo pela vol atual.

### 13. [Trend Carry Risk Regimes](2.Trend_Following_and_Carry/13.Trend_Carry_Risk_Regimes.ipynb)
Estratégia que combina tendência e carry condicionados a regimes de risco.
Faz o ajuste da posição utilizando o ajuste de vol tanto na média móvel quanto no carry, e utiliza a média das médias e média dos carrys.

### 14. [Spot Trend](2.Trend_Following_and_Carry/14.Spot_Trend.ipynb)
Modelo de tendência aplicado ao preço spot ou preço sintético.
Aplica a estratégia de médias móveis em cima de um spot sintético, sendo o preço ajustado subtraido do carry acumulado ao longo do tempo.

### 15. [Seasonal Carry](2.Trend_Following_and_Carry/15.Seasonal_Carry.ipynb)
Sinal de carry ajustado por padrões sazonais.
Melhora a estratégia 14, aplicando um filtro sazonal no carry antes de calcular o spot sintético.

### 16. [Trend and Carry Allocation](2.Trend_Following_and_Carry/16.Trend&Carry_Alocation.ipynb)
Estratégia de Trend e carry aplicada ao portfolio "Jumbo".
Não temos os dados de carry, então no script o portfolio tem apenas o SP500 e Gas.

### 17. [Normalized Trend](2.Trend_Following_and_Carry/17.Normalized_Trend.ipynb)
Sinal de tendência normalizado por volatilidade.
Aplica estratégia de médias móveis, porém calcula um "Preço Normalizado", sendo o acumulado dos pontos (retorno bruto) dividido pela volatilidade.

### 18. [Trend Following Assets](2.Trend_Following_and_Carry/18.Trend_Following_Assets.ipynb)
Aplicação das estratégias de trend e carry considerando setores.
calcula um indice dos setores a partir dos preços normalizados dos ativos e utiliza esse preço para ajustar as posições nas estratégias.

### 19. [Trend Following Relative Assets](2.Trend_Following_and_Carry/19.Trend_Following_Relative_Assets.ipynb)
Estratégia de tendência relativa entre ativos e indice do setor.
Uma melhora na estratégia 18, após calcular o indice setorial, calcula o retorno relativo de cada ativo e seu indice e usa esse retorno relativo para calcular as estratégias de trend e carry.

### 20. [Carry Relative Assets](2.Trend_Following_and_Carry/20.Carry_Relative_Assets.ipynb)
Estratégia de carry relativo entre ativos da mesma classe.
Semelhante a estratégia 19 rleative price, porém calcula a média do carry ara a classe do ativo e não do preço diretamente

---

## Advanced Directional

### 21. [Breakout](3.Advanced_Directional/21.Breakout%20copy.ipynb)
Estratégia de rompimento baseada nos maximos e minimos recentes.
faz um "forecast" usando o preço maximoe minico dos utimos x dias e tira  a média desse forecast para ajustar o tamanho da posição.


### 22. [Value](3.Advanced_Directional/22.Value.ipynb)
Modelo direcional baseado em valor, sendo o preço da relltivo dda classse do ativo.
O "Valor" usado para ajustar o tamanho da posição o negativo da outperformance do ativo e ele mesmo em um horinzonte de "x" dias. 

### 23. [Acceleration](3.Advanced_Directional/23.Accelaration.ipynb)
Estratégia focada na aceleração de tendência ou momentum da média móvel.
Utiliza a ideia de outpeformance, ou "Aceleração", sendo a diferença da média móvel de "x" dias do ativo e ela mesma em um horizonte de "k" dias para ajustar o tamanho da posição

### 24. [Skew](3.Advanced_Directional/24.Skew.ipynb)
Estratégia que utiliza assimetria (skew) da distribuição de retornos.
Mesma ideia da estratégia 23, porém utiliza o negativo da "skew" atual dos retornos do ativo, um rooling da skew dos retornos para ajustar a posição.

---

## Operador Total Return

### 25. [Momentum Double](Operador_TR/25.Momemtun_Double.ipynb)
Estratégia de momentum em dois horizontes temporais.
COmpara o ativo do mês anterior com o atual e do preço com a média móvel para ficar comprado.

### 26. [WeekDay](Operador_TR/26.WeekDay.ipynb)
Modelo baseado em efeitos de dia da semana.
Explora padrões de retorno de cada dia da semana.

### 27. [Roll Days Strategy](Operador_TR/27.roll_days_strategy.ipynb)
Estratégia que fica comprada quanto o retorno em janela móvel de "x" dias foi maior do na mesma janela em t-1 períodos

### 28. [N Days Down](Operador_TR/28.ndays_down.ipynb)
Compra após uma sequência de dias consecutivos de queda.

### 29. [Short After 1 Up](Operador_TR/29.short_after_1up.ipynb)
Venda após um dia de ala acima de 1% ou outro up trigger.

### 30. [First/Last Month Day](Operador_TR/30.first_last_month_day.ipynb)
Estratégia baseada no efeito do primeiro e último dia do mês, fica comprada apenas nesses dias.

### 31. [End Year](Operador_TR/31.end_year.ipynb)
Modelo focado em efeitos de fim de ano, fica comprado apenas em novembro e dezembro.

### 32. [After Week Move](Operador_TR/32.after_week_move.ipynb)
Estratégia que fica comprada na durante 1 semana, sempre que a semana anteriorrteve reetorno positivo.

### 33. [Loser Winner](Operador_TR/33.loser_winner.ipynb)
Modelo baseado na classificação de ativos vencedores e perdedores.
Estratégia que compara 2 ativos e fica comprado no que teve pior rretorno entre els no ultimos meses.

### 34. [MACD](Operador_TR/33.MACD.ipynb)
Estratégia direcional baseada no indicador MACD.
Utiliza cruzamentos e divergências para ficar comprado ou short, MACD classico.

### 35. [RSI](Operador_TR/35.RSI.ipynb)
Estratégia direcional baseada no indicador RSI (Relative Strength Index).
Utiliza níveis de sobrevenda (<30) e sobrecompra (>70) para gerar sinais de compra e venda, com reversão quando o RSI sai entra zonas extremas, entra na posição quando sai desse range e encerra quando entra de volta.

### 36. [BB_Band](Operador_TR/35.BB_Bands.ipynb)
Estratégia direcional baseada no indicador Bollinger Bands.
Utiliza as bandas superior e inferior (média móvel ± 2 desvios padrão) para identificar condições de sobrecompra/sobrevenda e explorar reversões de preço nas extremidades das bandas, entraa na posição quando o preço aza a banda e encerra quando ele voltta a pra dentro dela.

