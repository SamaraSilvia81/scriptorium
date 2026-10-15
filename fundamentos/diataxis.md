# Diátaxis: os quatro tipos de documentação

> **Status:** publicado
> **Tipo:** nota de estudo

## Pergunta principal

Por que tanta documentação parece confusa mesmo quando tem bastante conteúdo?

Uma resposta possível: ela tenta fazer tudo ao mesmo tempo. Ensina, explica, lista parâmetros e resolve problemas no mesmo texto — e acaba não fazendo nenhuma dessas coisas bem.

## O que é o Diátaxis

O [Diátaxis](https://diataxis.fr/) é um framework criado por Daniele Procida para organizar documentação técnica. A ideia central é que existem **quatro necessidades diferentes** de quem lê, e cada uma pede um tipo de texto.

| Tipo | Para quê | A pessoa está... | Pergunta que responde |
|:---|:---|:---|:---|
| **Tutorial** | Aprender fazendo | estudando | "Como eu começo?" |
| **Guia prático** (*how-to*) | Resolver um problema específico | trabalhando | "Como eu faço X?" |
| **Referência** | Consultar informação exata | trabalhando | "Qual é o parâmetro, o tipo, o retorno?" |
| **Explicação** | Entender o porquê | estudando | "Por que é assim?" |

Os quatro tipos se organizam em dois eixos: **ação × entendimento** e **estudo × trabalho**.

## Como reconhecer cada um

- **Tutorial** — conduz a pessoa do zero até um resultado que funciona. Não oferece escolhas nem desvia para explicações longas. O objetivo é a pessoa ter uma primeira experiência de sucesso.
- **Guia prático** — parte do princípio de que a pessoa já sabe o básico e tem um objetivo claro. É uma sequência de passos para chegar lá.
- **Referência** — descreve, não ensina. Precisa ser precisa, completa e organizada para consulta rápida. Documentação de API é o exemplo clássico.
- **Explicação** — dá contexto: decisões de design, alternativas consideradas, conceitos por trás. É onde cabe a discussão.

## Exemplo de aplicação

Pense num projeto com um único `README.md` enorme. Aplicando o Diátaxis:

- "Primeiros passos" vira um **tutorial**;
- "Como configurar autenticação" vira um **guia prático**;
- A lista de variáveis de ambiente vira **referência**;
- "Por que escolhemos essa arquitetura" vira **explicação** (ou um ADR — registro de decisão arquitetural).

O README passa a ser a porta de entrada que aponta para cada um.

## Limitações e questões em aberto

- Projetos pequenos não precisam de quatro seções separadas — às vezes um README bem dividido já aplica a ideia.
- Nem todo conteúdo cabe perfeitamente em uma caixa. O framework ajuda mais como lente para revisar do que como regra rígida.

## Referências

- [Diátaxis](https://diataxis.fr/) — Daniele Procida (site oficial).
