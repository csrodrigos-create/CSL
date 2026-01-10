# Guia de Uso das Estrategias

Este guia explica como rodar os notebooks e como usar os exemplos de estrategias, com exemplos separados por grupo:
- Estrategias do Robert Carver (Directional, Trend Following and Carry, Advanced Directional)
- Estrategias do Operador Total Return (Operador_TR)

## Antes de comecar (bem simples)

1) Tenha o Python instalado no computador.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2) Instale as bibliotecas do projeto:

```powershell
pip install -r requirements.txt
```

3) Abra o Jupyter para ver os notebooks:

```powershell
jupyter lab
```

## Onde ficam os dados

- Muitos notebooks buscam dados externos (ex.: `tvdatafeed`, `yfinance`, `ipeadatapy`).
- Alguns notebooks leem arquivos locais na pasta `_databases`.
- Se um notebook nao carregar dados, veja as primeiras celulas (ativos, contratos ou caminhos de arquivos).

## Como salvar novos dados (bem simples)

1) Crie um arquivo `.csv` e salve dentro da pasta `_databases`.
2) Use um nome simples (ex.: `meus_dados.csv`).
3) O arquivo precisa ter um cabecalho na primeira linha.

Exemplo de formato (CSV):

```csv
index,adjusted,underlying
2024-01-02,4800.0,4800.0
2024-01-03,4820.0,4820.0
```

Dica: se voce tiver dados em Excel, exporte para CSV e copie para `_databases`.

## Estrategias do Robert Carver (livro)

Os notebooks ficam nas pastas:
- `1.Directional`
- `2.Trend_Following_and_Carry`
- `3.Advanced_Directional`

Exemplos para comecar:
- `1.Directional/10.Basic_Carry.ipynb` - basic carry signal.
- `1.Directional/11.Basic_Carry&Trend.ipynb` - combines carry and trend.
- `2.Trend_Following_and_Carry/12.Adjusted_trend.ipynb` - adjusted trend signal.
- `2.Trend_Following_and_Carry/16.Trend&Carry_Alocation.ipynb` - signal allocation.
- `3.Advanced_Directional/21.Breakout copy.ipynb` - breakout strategy.

Como usar os exemplos (passo a passo, sem complicacao):
1) Abra o notebook.
2) Clique em "Run All" (Executar tudo).
3) Veja os graficos e o resumo de performance.
4) Se quiser, ajuste os parametros e rode novamente.

### Exemplo detalhado: 12.Adjusted_trend

O notebook usa dois ativos (SP500 e US10) e lê os dados da pasta `_databases`.

O que voce precisa ter:
1) Dois arquivos CSV:
   - `_databases/sp500.csv`
   - `_databases/us10.csv`
2) Cada arquivo precisa ter estas colunas:
   - `index` (data)
   - `adjusted` (preco ajustado)
   - `underlying` (preco do ativo)

Exemplo simples de arquivo (CSV):

```csv
index,adjusted,underlying
2024-01-02,4800.0,4800.0
2024-01-03,4820.0,4820.0
```

Como usar o exemplo:
1) Coloque os CSVs na pasta `_databases`.
2) Abra `2.Trend_Following_and_Carry/12.Adjusted_trend.ipynb`.
3) Clique em "Run All" (Executar tudo).
4) Veja o grafico de retorno acumulado e as estatisticas impressas.

Se quiser mudar os ativos:
1) Troque os nomes em `get_data_dict(['sp500','us10'])`.
2) Atualize `multipliers` e `cost_per_contract_dict` com os novos ativos.

## Estrategias do Operador Total Return (Operador_TR)

Os notebooks ficam na pasta `Operador_TR`.

Exemplos para comecar:
- `Operador_TR/25.Momemtun_Double.ipynb` - double timeframe momentum.
- `Operador_TR/26.WeekDay.ipynb` - day of week effect.
- `Operador_TR/27.roll_days_strategy.ipynb` - roll days effect.
- `Operador_TR/30.first_last_month_day.ipynb` - first/last month day effect.
- `Operador_TR/33.MACD.ipynb` - MACD signal.

Como usar os exemplos (passo a passo, sem complicacao):
1) Abra o notebook.
2) Clique em "Run All" (Executar tudo).
3) Confira o periodo de dados e o ativo usado.
4) Compare resultados mudando parametros e datas.
