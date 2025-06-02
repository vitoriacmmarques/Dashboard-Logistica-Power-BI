# Dashboard de Logística Internacional

Este repositório apresenta um projeto em Power BI voltado para análise de desempenho logístico em processos de importação. O objetivo é transformar dados brutos em visualizações claras que possibilitem o monitoramento de pedidos internacionais, status logístico e tempo de entrega por país.

## Objetivo do Projeto

Criar um painel interativo que forneça indicadores sobre o histórico de importações, como prazos, devoluções, performance por país e transportadora, facilitando a tomada de decisão em áreas de comércio exterior e logística.

## Fontes de Dados Utilizadas

- `Historico_Importacao.csv`  
  Contém o histórico operacional das importações, com colunas como:
  - Número do pedido
  - Cliente
  - País de origem
  - Transportadora
  - Data prevista de entrega
  - Data de entrega
  - Data de emissão da nota
  - Status do pedido
    

- `Bandeiras_Países.xlsx`  
  Planilha auxiliar utilizada para mapear os países com imagens de bandeiras e códigos, permitindo enriquecer visualmente os gráficos com ícones personalizados.

- `Cadastros_Comex.pdf`  
  Documento de apoio que detalha os conceitos, siglas e estrutura dos dados da área de comércio exterior, utilizado como referência para validação de colunas e criação de filtros inteligentes.

## Etapas do Projeto

### 1. Importação e Tratamento dos Dados
- Importação dos dados CSV e XLSX no Power BI
- Padronização de colunas de data e texto
- Criação de colunas calculadas para:
  - Dias de atraso
  - Entregas dentro ou fora do prazo
  - Pedidos devolvidos

### 2. Modelagem de Dados
- Relacionamento entre a tabela de histórico de importações e a tabela de países (para as bandeiras)
- Utilização de funções DAX para cálculo de indicadores:
  - Tempo médio de entrega
  - Taxa de devolução
  - Total de pedidos por país
  - Desempenho por transportadora

### 3. Criação das Visualizações
- Cartões de indicadores principais (total de pedidos, taxa de devolução, média de entrega)
- Gráfico de barras: pedidos por país
- Mapa geográfico com indicadores por país
- Matriz de análise por transportadora e status
- Segmentações por status, país e transportadora

### 4. Enriquecimento Visual
- Inclusão de bandeiras dos países nas tabelas e gráficos
- Formatação condicional para destacar entregas fora do prazo

## Tecnologias Utilizadas

- Power BI Desktop
- Power Query para ETL
- DAX para KPIs e medidas
- Visualizações nativas e mapas

## Demonstração


