# Mineração de Dados Eleitorais 2026

Projeto: análise descritiva à detecção de anomalias, usando dados reais e abertos do TSE (Eleições 2026).

## Estrutura do projeto

| Fase | Notebook | O que faz |
|---|---|---|
| 0 | `00_preparacao_dados.ipynb` | Lê os zips do TSE (baixados manualmente para `dados/`), filtra por cargo/UF, limpa e salva um dataset pronto em `dados/` |
| 1 | `01_analise_descritiva.ipynb` | Exploração ampla e sem viés: distribuições, outliers, proporções e dispersão de todas as variáveis relevantes (candidatos e bens) |
| 2 | `02_clusterizacao.ipynb` | K-Means e Bisecting K-Means |
| 2b | `02_clusterizacao_outros.ipynb` | DBSCAN e clusterização hierárquica (hclust) — mesma base e pergunta do notebook anterior |
| 3 | `03_regras_associacao.ipynb` | Regras de associação (Apriori) |
| 4 | `04_deteccao_anomalias.ipynb` | Detecção de anomalias |

## Fonte dos dados

Portal de dados abertos do TSE — Consulta de Candidatos e Bens de Candidatos, Eleições 2026 (`https://cdn.tse.jus.br/estatistica/sead/odsele/`).
