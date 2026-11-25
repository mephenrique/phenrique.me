---
title: "IA"
description: "Como a inteligência artificial é usada — e não usada — neste site, e como estas páginas foram feitas para serem lidas por agentes."
---

Vivemos em uma época em que a IA pode gerar uma quantidade enorme de texto sem praticamente nenhum esforço. Isso tem aplicações vantajosas, mas também levanta preocupações quando delegamos a essas ferramentas o conhecimento, o julgamento, a intencionalidade e o pensamento crítico humanos. Na verdade, essas qualidades se tornam mais valiosas do que nunca nesse cenário.[^slop]

Por isso, criei esta página para mostrar onde essas ferramentas estão presentes neste espaço e onde não estão.

## Como utilizo IA

::callout{type="note" title="Autoria estritamente humana"}
As ideias, a estrutura e os rascunhos de cada artigo, nota, resenha e opinião publicados neste site são estritamente meus. Posso usar IA para revisar, corrigir e sugerir melhorias de linguagem em trechos pontuais, mas eu decido o que aceitar e continuo responsável pelo texto final.
::

1. **Copiloto de engenharia**: Utilizo ferramentas de IA — LLMs e fluxos de programação agêntica — para explorar estruturas de código, gerar código boilerplate, prototipar estilos e layouts e acelerar refatorações. Continuo responsável por compreender e revisar o trabalho gerado por essas ferramentas.[^ghostty]
2. **Interlocutor intelectual**: Em estudos técnicos ou decisões arquiteturais, uso LLMs para pesquisar fontes, desafiar premissas, debater prós e contras e sugerir alternativas.
3. **Clareza e revisão**: Ocasionalmente, consulto modelos para apontar deslizes gramaticais ou sugerir formulações mais claras em português e inglês. Essas sugestões podem alterar trechos pontuais, mas as ideias e os rascunhos são meus, e eu reviso a redação final.

Especialmente em relação ao trabalho de engenharia de software, apoio-me bastante em agentes para as partes do trabalho que antes consumiam semanas ou meses. As primeiras versões deste site, por exemplo, foram feitas tradicionalmente, sem IA. Mas, com o avanço dos LLMs e dos agentes, a grande maioria do trabalho de desenvolvimento e evolução realizado aqui é feita por eles.

Embora essas ferramentas aumentem a produtividade, reconheço que é necessário prestar atenção ao que pode estar sendo deixado de lado ao delegar o trabalho, inclusive oportunidades de aprendizado.[^skills] Isso inclui ler, questionar e compreender os resultados antes de compartilhá-los.[^puget] Trato disso melhor no artigo ["Construindo software na era da IA"](/pt/writing/construindo-software-na-era-da-ia).

## Feito para ser lido por agentes

É curioso que, cada vez mais, o leitor daqui não seja uma pessoa com um navegador, mas um agente buscando uma página em nome de alguém. Como também prefiro acessar o texto puro de uma página web em muitas situações, resolvi atender aos dois públicos: cada página de conteúdo deste site tem uma gêmea em Markdown puro, no próprio endereço com `.md` ao final:

| Endereço                           | O que é                                          |
| :--------------------------------- | :----------------------------------------------- |
| [/pt/about.md](/pt/about.md)       | O autor deste site, em prosa                     |
| [/pt/work.md](/pt/work.md)         | Cargos, stack, formação                          |
| [/pt/reading.md](/pt/reading.md)   | O que estou lendo e o que já terminei            |
| [/pt/ai.md](/pt/ai.md)             | Esta página                                      |
| [/pt/colophon.md](/pt/colophon.md) | Como o site é feito                              |
| `/pt/writing/<slug>.md`            | Qualquer post, com suas notas de rodapé intactas |

Cada uma tem sua equivalente em inglês sem o prefixo. O [/llms.txt](/llms.txt) indexa todas elas, seguindo uma proposta para facilitar a descoberta de conteúdo por aplicações de LLM.[^llms] O sistema de design está publicado na íntegra em [/design.md](/design.md).

## Treinamento de modelos e a web aberta

::callout{type="insight" title="O bem comum da web aberta"}
Este site não bloqueia scrapers ou robôs de IA em seu `robots.txt`. Se modelos são treinados na web pública para expandir o conhecimento da humanidade, este espaço está aberto. Escritos humanos sinceros e bem pensados devem fazer parte do patrimônio comum de dados.
::

Tudo o que peço é o que a honestidade intelectual sempre exigiu: ao citar ideias ou trechos deste site, dê o devido crédito ao autor e inclua um link para a publicação original. A mesma cortesia vale para um agente escrevendo em nome de alguém.

[^slop]: Veja [No AI Slop Manifesto](https://www.slopmanifesto.com/): um manifesto que defende o julgamento humano, cuidado e responsabilidade pelo trabalho feito com IA.
[^ghostty]: A [política de uso de IA do Ghostty](https://github.com/ghostty-org/ghostty/blob/main/AI_POLICY.md) é um exemplo de projeto que acolhe a assistência de IA e espera que colaboradores compreendam suas contribuições e assumam responsabilidade por elas.
[^skills]: O [estudo da Anthropic sobre assistência de IA e formação de habilidades de programação](https://www.anthropic.com/research/AI-assistance-coding-skills) encontrou diferenças no aprendizado em uma tarefa específica, em parte conforme a maneira como os participantes usaram o assistente.
[^puget]: Em uma [publicação no X](https://x.com/JFPuget/status/2103081634140483943), @JFPuget relata sua preocupação com pessoas que compartilham resultados de agentes sem lê-los ou questioná-los.
[^llms]: A [proposta /llms.txt](https://llmstxt.org/) descreve um índice opcional em Markdown para acesso por aplicações de LLM; isso não garante que um agente o utilize.
