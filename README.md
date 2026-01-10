# Trading Strategies

Este repositório reúne os códigos em Python do curso **Operador Total Return** e estudos de estratégias quantitativas de trading.  
Veja `USAGE.md` para um guia simples de uso e exemplos por grupo de estrategias.
[References](#references).

## Summary <!-- no toc -->

- [Trading Strategies](#trading-strategies)
  - [Summary ](#summary-)
- [Uso](#uso)
- [Directional](#directional)
- [Trend Following and Carry](#trend-following-and-carry)
- [Advanced Directional](#advanced-directional)
- [Operador Total Return](#operador-total-return)
- [References](#references)


# Uso

Veja o guia simples de uso e exemplos em [Usage](USAGE.md)

# Directional

Notebooks da pasta `1.Directional` com estratégias direcionais clássicas e variações de tendência e carry.

- Buy and Hold — backtest de buy and hold em contratos de futuros. [1.Buy&Hold](1.Directional/1.Buy&Hold.ipynb)
- Buy and Hold with Risk Scaling — buy and hold com ajuste de risco fixo. [2.Buy&Hol_Risk_Scaling](1.Directional/2.Buy&Hol_Risk_Scaling.ipynb)
- Buy and Hold with Variable Risk Scaling — ajuste de risco variável ao longo do tempo. [3.Buy&Hold_Variable_Risk_Scaling](1.Directional/3.Buy&Hold_Variable_Risk_Scaling.ipynb)
- Buy and Hold Portfolio with Variable Risk — portfólio com escalonamento de risco variável. [4.Buy&Hold_Portifolio_Variable_Risk](1.Directional/4.Buy&Hold_Portifolio_Variable_Risk.ipynb)
- Trend Filter Long — filtro de tendência para posição somente long. [5.Trend_Filter_Long](1.Directional/5.Trend_Filter_Long.ipynb)
- Trend Filter Long and Short — filtro de tendência para posições long e short. [6.Trend_Filter_Long&Short](1.Directional/6.Trend_Filter_Long&Short.ipynb)
- Slow Trend Strength Filter — força de tendência com sinal mais lento. [7.Slow_Trend_Strength_Filter](1.Directional/7.Slow_Trend_Strength_Filter.ipynb)
- Fast Trend Strength Filter — força de tendência com sinal mais rápido. [8.Fast_Trend_Strength_Filter](1.Directional/8.Fast_Trend_Strength_Filter.ipynb)
- Multiple Trend Strength Filter — combinação de filtros de força de tendência. [9.Multiple_Trend_Strength_Filter](1.Directional/9.Multiple_Trend_Strength_Filter.ipynb)
- Basic Carry — estratégia básica de carry. [10.Basic_Carry](1.Directional/10.Basic_Carry.ipynb)
- Basic Carry and Trend — combinação simples de carry e tendência. [11.Basic_Carry&Trend](1.Directional/11.Basic_Carry&Trend.ipynb)

# Trend Following and Carry

Notebooks da pasta `2.Trend_Following_and_Carry` focados em modelos de tendência, carry e alocação entre sinais.

- Adjusted Trend — ajuste de sinal de tendência para reduzir ruído. [12.Adjusted_trend](2.Trend_Following_and_Carry/12.Adjusted_trend.ipynb)
- Trend Carry Risk Regimes — tendência e carry com regimes de risco. [13.Trend_Carry_Risk_Regimes](2.Trend_Following_and_Carry/13.Trend_Carry_Risk_Regimes.ipynb)
- Spot Trend — tendência usando preço spot/sintético. [14.Spot_Trend](2.Trend_Following_and_Carry/14.Spot_Trend.ipynb)
- Seasonal Carry — sinal de carry com sazonalidade. [15.Seasonal_Carry](2.Trend_Following_and_Carry/15.Seasonal_Carry.ipynb)
- Trend and Carry Allocation — alocação entre sinais de tendência e carry. [16.Trend&Carry_Alocation](2.Trend_Following_and_Carry/16.Trend&Carry_Alocation.ipynb)
- Normalized Trend — normalização do sinal de tendência. [17.Normalized_Trend](2.Trend_Following_and_Carry/17.Normalized_Trend.ipynb)
- Trend Following Assets — tendência aplicada por classe de ativo. [18.Trend_Following_Assets](2.Trend_Following_and_Carry/18.Trend_Following_Assets.ipynb)
- Trend Following Relative Assets — tendência relativa entre ativos. [19.Trend_Following_Relative_Assets](2.Trend_Following_and_Carry/19.Trend_Following_Relative_Assets.ipynb)
- Carry Relative Assets — carry relativo entre ativos. [20.Carry_Relative_Assets](2.Trend_Following_and_Carry/20.Carry_Relative_Assets.ipynb)

# Advanced Directional

Notebooks da pasta `3.Advanced_Directional` com sinais direcionais mais sofisticados.

- Breakout — estratégia de rompimento de faixa. [21.Breakout copy](3.Advanced_Directional/21.Breakout%20copy.ipynb)
- Value — estratégia baseada em valor relativo. [22.Value](3.Advanced_Directional/22.Value.ipynb)
- Acceleration — aceleração de tendência/momentum. [23.Accelaration](3.Advanced_Directional/23.Accelaration.ipynb)
- Skew — análise de assimetria (skew) no retorno. [24.Skew](3.Advanced_Directional/24.Skew.ipynb)

# Operador Total Return

Notebooks da pasta `Operador_TR` com estudos e estratégias do curso **Operador Total Return**.

- Momentum Double — estratégia de momentum em dois horizontes. [25.Momemtun_Double](Operador_TR/25.Momemtun_Double.ipynb)
- WeekDay — efeito de dia da semana. [26.WeekDay](Operador_TR/26.WeekDay.ipynb)
- Roll Days Strategy — padrão de rolagem de contratos. [27.roll_days_strategy](Operador_TR/27.roll_days_strategy.ipynb)
- N Days Down — compra após sequência de quedas. [28.ndays_down](Operador_TR/28.ndays_down.ipynb)
- Short After 1 Up — venda após um dia de alta. [29.short_after_1up](Operador_TR/29.short_after_1up.ipynb)
- First/Last Month Day — efeito do primeiro e último dia do mês. [30.first_last_month_day](Operador_TR/30.first_last_month_day.ipynb)
- End Year — efeito de fim de ano. [31.end_year](Operador_TR/31.end_year.ipynb)
- After Week Move — comportamento pós-movimento semanal. [32.after_week_move](Operador_TR/32.after_week_move.ipynb)
- Loser Winner — efeito de reversão ou continuidade (loser/winner). [33.loser_winner](Operador_TR/33.loser_winner.ipynb)
- MACD — sinal de tendência baseado no MACD. [33.MACD](Operador_TR/33.MACD.ipynb)

# References

- [Advanced Futures Trading Strategies: 30 fully tested strategies for multiple trading styles and time frames](https://a.co/d/hhuEtMJ) — Robert Carver
