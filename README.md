# ENEM 2025 — Pipeline de Dados

Projeto de Engenharia de Dados desenvolvido a partir dos microdados públicos do ENEM 2025, disponibilizados pelo INEP.

Este projeto é uma reconstrução para portfólio baseada em um trabalho que desenvolvi durante meu estágio no Ministério da Educação (MEC).

## Contexto

No projeto original, trabalhei com dados do ENEM de 2012 e 2022 com o objetivo de analisar e comparar indicadores ao longo de um período de dez anos.

Os dados eram disponibilizados em um ambiente PostgreSQL institucional estruturado em camadas Bronze, Silver e Gold.

A partir dos dados brutos disponíveis na camada Bronze, utilizei SQL e DBeaver para realizar a seleção, limpeza, tratamento e preparação das informações necessárias para a análise, trabalhando na transformação dos dados até a camada Gold.

Após a preparação dos dados, conectei o Power BI ao PostgreSQL e desenvolvi o dashboard, incluindo indicadores, filtros e visualizações. O layout do painel também foi desenvolvido por mim no Figma.

O dashboard final foi posteriormente disponibilizado em uma página institucional da STIC/MEC.

## Reconstrução do projeto

Como não possuo mais acesso ao ambiente e à infraestrutura utilizados no projeto original, este repositório apresenta uma reconstrução simplificada utilizando exclusivamente os microdados públicos do ENEM 2025.

O objetivo desta versão é reproduzir o processo de tratamento e preparação dos dados, com foco na arquitetura:

```text
Dados brutos
    |
    v
Bronze
    |
    v
Silver
    |
    v
Gold
```

O projeto será desenvolvido no Visual Studio Code.

O PostgreSQL será utilizado como banco de dados, enquanto scripts Python e consultas SQL serão utilizados para carregar, transformar e preparar os dados.

Nenhuma credencial, dado interno ou informação sobre a infraestrutura institucional do MEC é utilizada neste repositório.

## Objetivo

Construir um pipeline de dados para:

* carregar os microdados públicos do ENEM 2025;
* armazenar os dados originais na camada Bronze;
* realizar limpeza e tratamento dos dados;
* selecionar as informações relevantes para análise;
* estruturar os dados tratados na camada Silver;
* preparar os dados necessários para os indicadores na camada Gold;
* documentar as etapas e transformações realizadas;
* desenvolver no Figma um protótipo para apresentação dos indicadores.

## Arquitetura

```text
Microdados ENEM 2025
        |
        v
      Bronze
   Dados brutos
        |
        | SQL / Python
        v
      Silver
Limpeza e tratamento
        |
        | SQL / Python
        v
       Gold
Dados preparados
para indicadores
        |
        v
      Figma
Protótipo visual
```

### Bronze

Armazena os dados provenientes da fonte original com o mínimo possível de alterações.

### Silver

Contém os dados após as etapas de limpeza, tratamento, seleção e padronização.

### Gold

Contém os dados preparados para análise e geração dos indicadores utilizados no protótipo.

## Tecnologias

### Reconstrução atual

* Python
* PostgreSQL
* SQL
* Visual Studio Code
* Figma
* Git
* GitHub

### Projeto original

* PostgreSQL
* SQL
* DBeaver
* Power BI
* Figma

## Fonte dos dados

Os dados utilizados neste projeto são provenientes dos Microdados do ENEM 2025, disponibilizados publicamente pelo Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (INEP).

Os arquivos originais não serão armazenados neste repositório devido ao seu tamanho. O processo para obtenção e carregamento dos dados será documentado no projeto.

## Estrutura do projeto

```text
enem-2025-pipeline/
|
|-- dados/
|-- sql/
|   |-- bronze/
|   |-- silver/
|   `-- gold/
|
|-- src/
|-- docs/
|-- imagens/
|-- .gitignore
`-- README.md
```

A estrutura poderá ser atualizada conforme o desenvolvimento do projeto.

## Protótipo visual

Após a preparação dos dados na camada Gold, será desenvolvido um protótipo no Figma para demonstrar uma possível apresentação dos indicadores.

O Power BI fez parte do projeto original desenvolvido no MEC, mas não será utilizado nesta reconstrução.

## Status

Projeto em desenvolvimento.
