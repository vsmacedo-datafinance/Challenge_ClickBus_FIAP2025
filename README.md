# Challenge ClickBus — FIAP 2025

Projeto de ciência de dados desenvolvido para a ClickBus com dados reais 
de ~1,7 milhões de transações (set/2013 – abr/2024).

## Desafios resolvidos
1. **Segmentação de clientes** — K-Means com 4 clusters (Ocasionais, Frequentes, Recorrentes e VIPs)
2. **Previsão de compra em 30 dias** — XGBoost | ROC AUC: 0.89 | F1: 0.47
3. **Previsão do próximo trecho** — LightGBM multiclasse | F1-macro: 0.54

## Decisões técnicas relevantes
- Divisão temporal dos dados (sem data leakage)
- Variável COVID com datas oficiais OMS/OPAS (mar/2020 – mai/2023)
- Delta de 5 dias para compras relacionadas a feriados
- SMOTE para balanceamento de classes

## Arquitetura
| Camada | Arquivo | Conteúdo |
|--------|---------|----------|
| Bronze | `clickbus_bronze.parquet` | Dado bruto original |
| Prata  | `clickbus_prata.parquet`  | Limpo, decodificado |
| Ouro   | `clickbus_ouro.parquet`   | Features + modelo |

## Stack
Python · XGBoost · LightGBM · Scikit-Learn · SMOTE · Pandas

## Equipe — FIAP
Bruno Rosa · Danilo Alves · Fred Sousa · Luana Ferreira · Vinicius Macedo
