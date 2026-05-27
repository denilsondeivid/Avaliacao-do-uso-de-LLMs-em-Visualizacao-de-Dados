# Contexto e insights da pesquisa

Esta pagina resume, em linguagem direta, o contexto do trabalho e os principais pontos de analise e discussao observados ate o momento.

## Resumo da introducao

A pesquisa parte de um problema central: visualizacoes de dados mal construidas podem comprometer a interpretacao de informacoes, mesmo quando os dados subjacentes estao corretos. Em contextos cientificos, educacionais e profissionais, esse tipo de falha pode induzir leituras equivocadas, prejudicar comparacoes e enfraquecer a comunicacao visual.

Ao mesmo tempo, a expansao recente dos modelos de linguagem de grande escala abriu uma oportunidade de investigacao relevante: ate que ponto essas ferramentas conseguem analisar visualizacoes de dados com base em boas praticas da literatura? O trabalho se insere justamente nesse ponto, avaliando se LLMs conseguem reconhecer erros visuais recorrentes e, em um segundo momento, propor versoes corrigidas sem introduzir novos problemas.

O estudo foi construido com base em referencias consolidadas de visualizacao de dados e em uma avaliacao empirica com diferentes modelos e tecnicas de prompting. A proposta nao e apenas verificar se os modelos respondem algo plausivel, mas observar se eles conseguem identificar o erro-alvo, justificar a analise e contribuir com uma resposta util para a melhoria do grafico.

## Resumo da analise e discussao dos resultados

Os resultados reunidos ate aqui indicam que as LLMs possuem potencial real para apoiar tarefas de avaliacao e melhoria de visualizacoes de dados, mas esse potencial nao aparece de forma uniforme entre os modelos. O comportamento observado sugere que o desempenho depende tanto do modelo utilizado quanto da estrategia de prompting adotada.

Na etapa de identificacao de erros, os achados apontam que ChatGPT e Claude se destacam em robustez geral, enquanto o DeepSeek apresenta desempenho inferior e maior instabilidade qualitativa, inclusive com ocorrencia de respostas alucinatorias. Isso sugere que, para tarefas de leitura visual com criterio teorico, nem todo modelo generalista responde com o mesmo nivel de consistencia.

Outro ponto importante da discussao e que a tecnica de prompt nao produz ganhos universais. Em vez de existir uma estrategia unica claramente superior para todos os casos, os resultados sugerem que a eficacia do zero-shot, few-shot ou chain-of-thought varia conforme o modelo e a tarefa. Isso reforca a ideia de que comparacoes entre LLMs em visualizacao precisam considerar nao apenas o modelo, mas tambem a forma como a interacao e estruturada.

Na etapa de correcao de erros, o desempenho geral dos modelos selecionados foi alto, com indicios de maior consistencia qualitativa por parte do ChatGPT. Esse resultado e relevante porque mostra que, quando a tarefa passa da identificacao para a proposicao de uma melhoria, algumas LLMs conseguem manter bom desempenho e ainda produzir saidas visualmente mais adequadas.

Em conjunto, a discussao aponta tres leituras principais:

- as LLMs ja demonstram utilidade pratica para apoiar revisao de visualizacoes de dados;
- a confiabilidade ainda varia bastante entre modelos e tecnicas de prompt;
- a avaliacao humana continua importante, especialmente para capturar nuances de justificativa, adequacao visual e presenca de novos erros.

## Leitura interpretativa

De forma geral, o material do repositorio sustenta a ideia de que LLMs podem funcionar como apoio em tarefas de diagnostico e melhoria de graficos, mas ainda nao como substitutas plenas de avaliacao especializada. O valor mais evidente dos modelos aparece quando eles contribuem com triagem, explicacao inicial e sugestoes de melhoria, enquanto a validacao final ainda depende de criterio humano e referencia teorica consistente.
