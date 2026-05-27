# Avaliacao do uso de LLMs em Visualizacao de Dados

Este repositorio organiza os materiais da pesquisa de TCC sobre o uso de modelos de linguagem de grande porte na analise de graficos, com foco em duas frentes experimentais:

- identificacao de erros de visualizacao;
- correcao de erros de visualizacao.

A pesquisa esta em andamento. O repositorio foi estruturado para separar claramente os dados brutos, os notebooks, os resultados visuais e o material textual do TCC, facilitando a leitura, a reproducao e a expansao futura do trabalho.

## Sintese da pesquisa

O estudo investiga como diferentes LLMs respondem a tarefas relacionadas a visualizacao de dados em dois cenarios complementares:

1. identificar erros presentes em graficos;
2. propor ou verificar correcoes para esses erros.

Os experimentos usam imagens-base de graficos, respostas textuais de diferentes modelos, uma planilha de mapeamento da avaliacao grafica e notebooks de analise para consolidar metricas e gerar figuras comparativas.

## Onde esta cada etapa da pesquisa

- `experimentos/identificacao-de-erros/`: materiais da etapa de identificacao de erros, incluindo respostas dos modelos, notebook principal e figuras de resultado.
- `experimentos/correcao-de-erros/`: materiais da etapa de correcao de erros, incluindo respostas dos modelos, notebook da etapa e figuras associadas.
- `dados/brutos/`: planilha central utilizada como base de avaliacao.
- `assets/imagens-base/`: conjunto de graficos-base estudados na pesquisa.
- `docs/`: documentacao textual de apoio, incluindo metodologia, status da pesquisa e guia de navegacao.
- `manuscrito/`: versoes do TCC e materiais de apoio a escrita academica.
- `archive/`: observacoes sobre a origem dos arquivos e referencias ao material bruto reorganizado.

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

## Fluxo geral dos materiais

1. `assets/imagens-base/` concentra os graficos originais usados como objeto de estudo.
2. `dados/brutos/` guarda a planilha principal de avaliacao.
3. Cada pasta dentro de `experimentos/` separa os artefatos da etapa correspondente.
4. Em cada experimento, os dados brutos das respostas dos modelos ficam em `dados/brutos/respostas-llms/`.
5. Os notebooks da etapa ficam em `notebooks/`.
6. As figuras e saidas associadas a cada etapa ficam em `resultados/`.
7. O material textual do trabalho academico fica em `manuscrito/`.

## Etapas experimentais

### Identificacao de erros

Esta etapa reune as respostas de multiplos modelos em diferentes rodadas e tecnicas de prompting para analisar a capacidade de detectar problemas de visualizacao em graficos.

Local principal:
- `experimentos/identificacao-de-erros/`

Conteudo esperado nessa etapa:
- respostas brutas por modelo e rodada;
- notebook de consolidacao e analise;
- figuras geradas a partir das avaliacoes;
- espaco para dados processados e tabelas derivadas.

### Correcao de erros

Esta etapa reune os materiais ligados a analise e proposta de correcao de erros de visualizacao, incluindo verificacao da qualidade das respostas e resultados comparativos.

Local principal:
- `experimentos/correcao-de-erros/`

Conteudo esperado nessa etapa:
- respostas brutas dos modelos;
- notebook de analise da etapa;
- figuras de apoio e resultados gerados;
- espaco para tabelas e consolidacoes futuras.

## Documentacao complementar

- `docs/visao-geral.md`: resumo do repositorio e dos seus blocos principais.
- `docs/metodologia.md`: descricao resumida da logica metodologica da pesquisa.
- `docs/status-da-pesquisa.md`: registro do estagio atual da organizacao e da pesquisa.
- `docs/organizacao-do-repositorio.md`: guia rapido de navegacao pelas pastas.

## Observacoes

- Os nomes das pastas e arquivos foram normalizados para facilitar navegacao, versionamento e reproducao.
- O material original local foi reorganizado sem incluir o arquivo compactado bruto no versionamento.
- Como a pesquisa esta em andamento, novas rodadas, modelos, tabelas e figuras podem ser adicionados mantendo a mesma estrutura.
