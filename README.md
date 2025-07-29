# Business Intelligence – Airbnb NYC

Análise exploratória e estratégica de dados públicos do Airbnb em Nova York. O objetivo é identificar padrões de performance, ocupação e precificação para orientar hosts na otimização de suas receitas e estratégias de anúncio.

## Visão Geral

O mercado de locações de curta duração em NYC é altamente competitivo. Este projeto analisa mais de 48 mil acomodações com foco em fatores que influenciam a receita por noite (RevPAR), taxa de ocupação, impacto do preço e avaliações, além do perfil dos hosts.

## Problema Central

Hosts precisam tomar decisões estratégicas com base em dados. A análise busca responder:

- Quais regiões e tipos de acomodação geram mais receita?
- O preço impacta diretamente a ocupação?
- Hosts com múltiplos imóveis têm melhor desempenho por acomodação?
- A estadia mínima e as avaliações influenciam a performance?

## Ferramentas e Tecnologias

- **SQL + BigQuery**
- **Python (pandas, matplotlib, seaborn)**
- **VS Code**
- **Power BI**

## Estrutura do Repositório
- `/dataset`: Base de dados original e tratada (CSV).
  - /dados_brutos
  - /dados_tratados
- `/documentacao`: Documentos técnicos do projeto.
  - `apresentacao_churn_colaboradores.pdf`: Metodologia, Tratamento de Dados e Insights.
  - `ficha_tecnica_churn_colaboradores.pdf`: Insights e Recomendações.
- `rh_churn.ipynb`: Notebook com EDA, engenharia de atributos e modelagem preditiva.
- `requirements.txt`: Bibliotecas utilizadas.

## Metodologia

### Pré-processamento e Limpeza

- Remoção de inconsistências (tipagem, nulos, duplicados)
- Conversão de variáveis e validação de chaves primárias

### Carga no BigQuery

- Importação de dados já tratados
- Otimização de estrutura e tipos para análises via SQL

### Análise Exploratória (EDA)

- Boxplots e histogramas para identificação de outliers
- Correlação entre variáveis
- Criação de faixas categóricas com base em lógica de negócio

### Dashboard Power BI

- KPIs: RevPAR, Ocupação, Preço Médio, Total de Anúncios
- Análises cruzadas por região, tipo de acomodação, faixa de preço, reviews e estadia mínima

## Principais Insights Estratégicos

- **Manhattan e apartamentos inteiros** geram maior RevPAR (até $107 por noite).
- **Preços até $100** aumentam ocupação (até 61%).
- **Hosts com apenas 1 imóvel** têm o melhor desempenho por unidade (RevPAR médio de $96).
- **Estadias mínimas de 3 a 10 noites** maximizam a taxa de ocupação.
- **Avaliações recentes** aumentam a confiança dos hóspedes e a ocupação (até 57%).

## Recomendações para Hosts

- Ofereça o imóvel inteiro, preferencialmente em Manhattan ou Brooklyn.
- Mantenha preços competitivos (até $100) em imóveis padrão.
- Configure estadias mínimas entre 3 e 10 noites.
- Busque avaliações nas primeiras reservas.
- Invista em fotos, descrição clara e atendimento de qualidade.

## Analista de Dados

**Cristiane Thiel**  
🌐 [https://cristianethiel.com.br/](https://cristianethiel.com.br/)  
🔗 [https://www.linkedin.com/in/cristianethiel/](https://www.linkedin.com/in/cristianethiel/)

