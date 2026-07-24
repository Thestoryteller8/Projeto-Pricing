[README.md](https://github.com/user-attachments/files/30359453/README.md)
# Precificação de Crédito Orientada por Dados

Projeto de ciência de dados aplicado a um problema de **precificação de crédito**: construção de
uma política de taxas diferenciada por risco a partir de três bases (operações de crédito,
inadimplência histórica e conversão comercial).

## O que este projeto cobre

- Leitura, limpeza e padronização de dados (incluindo tratamento de inconsistências cadastrais)
- Normalização de tabelas dinâmicas/pivotadas para formato tabular (`long format`)
- Engenharia de atributos (faixas de risco, prazo, valor, relacionamento)
- Análise exploratória com foco em poder de discriminação de variáveis sobre inadimplência
- Modelagem do custo de risco de crédito a partir de premissas de maturação da inadimplência
- Construção de uma matriz de precificação por segmento (risco x faixa de valor)
- Estimativa de conversão esperada e avaliação econômica da política proposta

## Como reproduzir

Este repositório **não inclui os arquivos de dados originais** (fornecidos em um contexto de
processo seletivo, sob uso restrito). Para rodar o notebook localmente:

1. Coloque os arquivos `Operacoes_Credito_1.xlsx`, `Inadimplencia_1.xlsx` e `Conversão_1.xlsx`
   em uma pasta `dados/` na raiz do projeto.
2. Instale as dependências: `pip install pandas numpy matplotlib openpyxl jupyter`
3. Rode `jupyter notebook precificacao_credito_portfolio.ipynb`

## Estrutura do notebook

| Seção | Conteúdo |
|---|---|
| 1–9 | Preparação e integração dos dados |
| 10 | Análise exploratória e seleção de variáveis |
| 11 | Premissas financeiras e construção da política |
| 12 | Resultados (volume, conversão, resultado esperado) |
| 13 | Conclusão e recomendações |
