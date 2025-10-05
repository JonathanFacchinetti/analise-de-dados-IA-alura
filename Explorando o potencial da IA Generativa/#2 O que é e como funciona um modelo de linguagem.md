# O que é e como funciona um modelo de linguagem?

Esta aula introduz o conceito fundamental por trás de ferramentas como
ChatGPT e Gemini, explicando o que são os modelos de linguagem e como
eles operam.

O ponto de partida é o **Processamento de Linguagem Natural (NLP)**, uma
área da inteligência artificial cujo objetivo é permitir que máquinas e
seres humanos se comuniquem usando a linguagem do dia a dia. Em vez de
escrever um código em linguagem de programação, podemos simplesmente
conversar com o computador (texto ou voz) e ele será capaz de
interpretar e responder.

## Como os modelos aprendem a linguagem?

O funcionamento dos modelos de linguagem é baseado em **identificar
padrões em enormes volumes de dados textuais**, como grande parte do
conteúdo disponível na internet.

Eles passam por três mecanismos principais de aprendizado:

-   **Aprendizado de Padrões:** o modelo reconhece estruturas
    gramaticais e semânticas.\
    *Exemplo:* em português, o verbo *gostar* costuma ser seguido da
    preposição *de* ("gosto de pizza"), mas em inglês esse padrão não
    existe ("I like pizza").\
    Assim, o modelo aprende as nuances de cada idioma e consegue gerar
    frases naturais.

-   **Cálculo de Probabilidade:** a tarefa central é prever a próxima
    palavra em uma sequência de texto. Funciona como uma versão
    extremamente sofisticada do autocompletar do celular.\
    *Exemplo:* dado o início "Eu gosto de", o modelo pode calcular
    probabilidades:\
    *chocolate -- 0.35, viajar -- 0.25, ler -- 0.20*.\
    Se o usuário completa com *chocolate*, o modelo recalcula as
    próximas probabilidades (como *porque* ou *e*).

-   **Generalização:** os modelos não decoram frases, mas aprendem
    padrões estatísticos. Isso os torna capazes de responder a frases
    nunca vistas, mas que seguem estruturas similares.

## A revolução: memória contextual

O grande avanço que permitiu aos modelos se tornarem assistentes
conversacionais foi a **capacidade de manter o contexto dentro de uma
conversa**. Antes, as interações eram independentes. Agora, o modelo
consegue interpretar pronomes, referências e continuidade.

*Exemplo:*\
Usuário: "Qual é a fórmula do Excel para encontrar o maior valor?"\
IA: "MAX"\
Usuário: "Me dê um exemplo dessa fórmula."\
O modelo entende que *dessa* se refere a *MAX* e gera uma resposta
consistente.\
Essa habilidade tornou a interação fluida, possibilitando que modelos
fossem usados como assistentes virtuais.

------------------------------------------------------------------------