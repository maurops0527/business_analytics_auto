# Projeto 2 — Business Analytics | Carteira Auto

**Projeto independente | Seguros Auto | Business Analytics | Pricing | R**

## Objetivo

Analisar a deterioração da sinistralidade de uma carteira de Seguro Auto, decompondo o resultado em **prêmio, frequência, severidade e composição dos sinistros**, e traduzindo os achados em hipóteses e recomendações para áreas de negócio.

## Pergunta de negócio

A carteira apresenta deterioração crescente da sinistralidade. O objetivo do estudo é entender **o que está pressionando o resultado**, quais componentes merecem investigação prioritária e quais análises adicionais podem apoiar decisões de Pricing, Sinistros e Comercial.

## Abordagem

1. Evolução de prêmio, sinistros, salvados e sinistralidade.
2. Decomposição entre frequência e severidade.
3. Análise de quantidade, custo total e custo médio por tipo de sinistro.
4. Teste de estresse sobre custos médios.
5. Avaliação das hipóteses relacionadas a inflação setorial.
6. Investigação de canais de distribuição.
7. Avaliação da deterioração por safra.
8. Transformação dos achados em perguntas e recomendações para as áreas envolvidas.
9. Proposta de aprofundamento com modelagem de severidade, séries temporais e Machine Learning.

## Principais resultados documentados no case

- Sinistralidade bruta: **60,83% em janeiro → 69,83% em junho**.
- Sinistralidade líquida de salvados: **56,17% → 65,69%**.
- Quantidade de sinistros: **5.220 → 4.930**, queda no período.
- Custo médio por sinistro: **R$ 13.980 → R$ 16.430**, aumento no período.
- No teste de estresse com redução de 20% do custo médio, os impactos documentados foram **3,97 p.p. para Colisão Parcial, 3,62 p.p. para Perda Total e 3,10 p.p. para Roubo/Furto**.
- O material do case aponta PT e RF como fortes indícios de deterioração pela magnitude dos custos médios e participação no custo total, mas ressalta a necessidade de histórico mensal para uma conclusão mais robusta.

## Estrutura

```text
├── README.md
├── data/
│   ├── carteira_auto.csv
│   ├── case_indicadores_mensais.csv
│   └── case_teste_estresse.csv
├── docs/
│   ├── data_dictionary.md
│   ├── enunciados.md
│   ├── memoria_calculo.xlsx
│   ├── portfolio_page.md
│   ├── resolucoes.md
│   └── resumo_executivo.md
├── outputs/
│   └── README.md
└── R/
    ├── 01_analise_exploratoria.R
    ├── 02_analise_severidade.R
    ├── 03_teste_estresse.R
    └── 04_canais_e_safras.R
```

## Observação metodológica

A base `carteira_auto.csv` é a base fornecida para o case. Os arquivos `case_indicadores_mensais.csv` e `case_teste_estresse.csv` são **tabelas derivadas da memória de cálculo original**, criadas para tornar explícitos os inputs agregados utilizados nas respostas.

Os scripts em `R/` são uma organização/reconstrução da lógica analítica do material fornecido; não são apresentados como os arquivos R originais do case.

## Documentação

- [Enunciado](docs/enunciados.md)
- [Resoluções](docs/resolucoes.md)
- [Resumo Executivo](docs/resumo_executivo.md)
- [Dicionário de Dados](docs/data_dictionary.md)
- [Página para CV/LinkedIn](docs/portfolio_page.md)

## Tecnologias

**R | Excel | Business Analytics | Insurance Pricing | Data Analysis**
