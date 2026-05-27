# Avaliacao do uso de LLMs em Visualizacao de Dados

Este repositorio apresenta os materiais do TCC sobre o uso de modelos de linguagem de grande porte na analise de visualizacoes de dados. A pesquisa foi organizada para mostrar com clareza:

- quais graficos foram estudados;
- como os modelos foram avaliados;
- onde estao os resultados de cada etapa;
- como acompanhar a evolucao do trabalho.

Atualmente a pesquisa esta estruturada em duas frentes experimentais:

1. identificacao de erros de visualizacao;
2. correcao de erros de visualizacao.

## Sintese

O estudo investiga como diferentes LLMs respondem a tarefas relacionadas a visualizacao de dados em dois cenarios complementares:

- detectar problemas visuais presentes em graficos;
- propor ou verificar correcoes para esses problemas.

Os experimentos combinam imagens-base, respostas textuais de diferentes modelos, planilha de avaliacao, notebooks analiticos e figuras comparativas produzidas ao longo da pesquisa.

## Leitura rapida

Se voce quer entender o repositorio em poucos minutos, siga esta ordem:

1. leia este `README.md`;
2. consulte [`docs/guia-de-leitura.md`](docs/guia-de-leitura.md);
3. veja a etapa de [`identificacao-de-erros`](experimentos/identificacao-de-erros/README.md);
4. veja a etapa de [`correcao-de-erros`](experimentos/correcao-de-erros/README.md);
5. consulte o material academico em [`manuscrito/`](manuscrito/README.md).

## Onde esta cada parte da pesquisa

| Bloco | Funcao |
|---|---|
| [`assets/imagens-base/`](assets/imagens-base/) | Graficos-base estudados na pesquisa |
| [`dados/brutos/`](dados/brutos/) | Planilha central de avaliacao |
| [`experimentos/identificacao-de-erros/`](experimentos/identificacao-de-erros/README.md) | Etapa de identificacao de erros, com respostas, notebook e figuras |
| [`experimentos/correcao-de-erros/`](experimentos/correcao-de-erros/README.md) | Etapa de correcao de erros, com respostas, notebook e figuras |
| [`docs/`](docs/) | Documentacao de apoio, navegacao e status da pesquisa |
| [`manuscrito/`](manuscrito/README.md) | TCC em PDF e materiais de apoio academico |
| [`archive/`](archive/origem/README.md) | Registro da origem e reorganizacao do material |

## Estrutura do repositorio

```text
.
|-- README.md
|-- docs/
|-- dados/
|   `-- brutos/
|-- assets/
|   `-- imagens-base/
|-- experimentos/
|   |-- identificacao-de-erros/
|   `-- correcao-de-erros/
|-- manuscrito/
`-- archive/
```

## Fluxo dos materiais

1. os graficos-base ficam em `assets/imagens-base/`;
2. a planilha principal fica em `dados/brutos/`;
3. cada etapa experimental possui sua propria pasta em `experimentos/`;
4. dentro de cada etapa, as respostas brutas ficam em `dados/brutos/respostas-llms/`;
5. os notebooks ficam em `notebooks/`;
6. as figuras e saidas ficam em `resultados/`;
7. o material academico fica em `manuscrito/`.

## Etapas experimentais

### Identificacao de erros

Esta etapa analisa a capacidade dos modelos de identificar erros de visualizacao em graficos. Ela concentra multiplas rodadas, tecnicas de prompting e respostas de diferentes LLMs.

- pasta principal: [`experimentos/identificacao-de-erros/`](experimentos/identificacao-de-erros/README.md)
- modelos presentes: ChatGPT, Claude, DeepSeek e Gemini
- materiais principais: respostas por rodada, notebook analitico e figuras de resultados

### Correcao de erros

Esta etapa concentra a analise e verificacao de respostas voltadas a correcao de problemas de visualizacao, incluindo a proposta de versoes corrigidas dos graficos.

- pasta principal: [`experimentos/correcao-de-erros/`](experimentos/correcao-de-erros/README.md)
- modelos presentes: ChatGPT e Claude
- materiais principais: respostas brutas, notebook da etapa e figuras associadas

## Destaques visuais

### Graficos-base

| Exemplo 1 | Exemplo 2 |
|---|---|
| ![](assets/imagens-base/grafico-01.jpeg) | ![](assets/imagens-base/grafico-02.jpeg) |

### Saidas da etapa de identificacao

| Figura 1 | Figura 2 |
|---|---|
| ![](experimentos/identificacao-de-erros/resultados/figuras/figura-identificacao-01.png) | ![](experimentos/identificacao-de-erros/resultados/figuras/figura-identificacao-02.png) |

### Saidas da etapa de correcao

| Figura 1 | Figura 2 |
|---|---|
| ![](experimentos/correcao-de-erros/resultados/figuras/figura-correcao-01.png) | ![](experimentos/correcao-de-erros/resultados/figuras/figura-correcao-02.png) |

Mais referencias visuais estao em [`docs/resultados-em-destaque.md`](docs/resultados-em-destaque.md).

## Documentacao complementar

- [`docs/guia-de-leitura.md`](docs/guia-de-leitura.md): percurso sugerido para ler o repositorio
- [`docs/visao-geral.md`](docs/visao-geral.md): resumo dos blocos principais
- [`docs/metodologia.md`](docs/metodologia.md): descricao resumida da logica metodologica
- [`docs/status-da-pesquisa.md`](docs/status-da-pesquisa.md): estado atual da pesquisa
- [`docs/organizacao-do-repositorio.md`](docs/organizacao-do-repositorio.md): mapa rapido das pastas
- [`docs/resultados-em-destaque.md`](docs/resultados-em-destaque.md): galeria comentada de figuras

## Status atual

- a organizacao do repositorio ja reflete o fluxo da pesquisa;
- a etapa de identificacao de erros esta mais ampla em modelos e rodadas;
- a etapa de correcao de erros esta organizada e pronta para expansao;
- novas tabelas, rodadas e consolidacoes podem ser adicionadas sem alterar a logica principal.

## Observacoes

- os nomes das pastas e arquivos foram normalizados para facilitar navegacao, versionamento e reproducao;
- o material original local foi reorganizado sem incluir o arquivo compactado bruto no versionamento;
- como a pesquisa esta em andamento, o repositorio foi preparado para crescimento incremental.
