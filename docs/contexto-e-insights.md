# Contexto e insights da pesquisa

Esta página resume, em linguagem direta, o contexto do trabalho e os principais pontos de análise e discussão observados até o momento.

## Resumo da introdução

A pesquisa parte de um problema central: visualizações de dados mal construídas podem comprometer a interpretação de informações, mesmo quando os dados subjacentes estão corretos. Em contextos científicos, educacionais e profissionais, esse tipo de falha pode induzir leituras equivocadas, prejudicar comparações e enfraquecer a comunicação visual.

Ao mesmo tempo, a expansão recente dos modelos de linguagem de grande escala abriu uma oportunidade de investigação relevante: até que ponto essas ferramentas conseguem analisar visualizações de dados com base em boas práticas da literatura? O trabalho se insere justamente nesse ponto, avaliando se VLMs conseguem reconhecer erros visuais recorrentes e, em um segundo momento, propor versões corrigidas sem introduzir novos problemas.

O estudo foi construído com base em referências consolidadas de visualização de dados e em uma avaliação empírica com diferentes modelos e técnicas de prompt. A proposta não é apenas verificar se os modelos respondem algo plausível, mas observar se eles conseguem identificar o erro-alvo, justificar a análise e contribuir com uma resposta útil para a melhoria do gráfico.

## Resumo da análise e discussão dos resultados

Os resultados reunidos até aqui indicam que as VLMs possuem potencial real para apoiar tarefas de avaliação e melhoria de visualizações de dados, mas esse potencial não aparece de forma uniforme entre os modelos. O comportamento observado sugere que o desempenho depende tanto do modelo utilizado quanto da estratégia de prompting adotada.

Na etapa de identificação de erros, os achados apontam que GPT-5.4 e Claude se destacam em robustez geral, enquanto o DeepSeek apresenta desempenho inferior e maior instabilidade qualitativa, inclusive com ocorrência de respostas alucinatórias. Isso sugere que, para tarefas de leitura visual com critério teórico, nem todo modelo generalista responde com o mesmo nível de consistência.

Outro ponto importante da discussão é que a técnica de prompt não produz ganhos universais. Em vez de existir uma estratégia única claramente superior para todos os casos, os resultados sugerem que a eficácia do zero-shot, few-shot ou chain-of-thought varia conforme o modelo e a tarefa. Isso reforça a ideia de que comparações entre VLMs em visualização precisam considerar não apenas o modelo, mas também a forma como a interação é estruturada.

Na etapa de correção de erros, o desempenho geral dos modelos selecionados foi alto, com indícios de maior consistência qualitativa por parte do GPT-5.4. Esse resultado é relevante porque mostra que, quando a tarefa passa da identificação para a proposição de uma melhoria, algumas VLMs conseguem manter bom desempenho e ainda produzir saídas visualmente mais adequadas.

Em conjunto, a discussão aponta três leituras principais:

- as VLMs já demonstram utilidade prática para apoiar revisão de visualizações de dados;
- a confiabilidade ainda varia bastante entre modelos e técnicas de prompt;
- a avaliação humana continua importante, especialmente para capturar nuances de justificativa, adequação visual e presença de novos erros.

## Leitura interpretativa

De forma geral, o material do repositório sustenta a ideia de que VLMs podem funcionar como apoio em tarefas de diagnóstico e melhoria de gráficos, mas ainda não como substitutas plenas de avaliação especializada. O valor mais evidente dos modelos aparece quando eles contribuem com triagem, explicação inicial e sugestões de melhoria, enquanto a validação final ainda depende de critério humano e referência teórica consistente.
