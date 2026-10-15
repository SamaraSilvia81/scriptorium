# Pinterest e a adoção de docs-as-code

> **Status:** publicado
> **Tipo:** registro de caso

## Contexto

O time de engenharia do Pinterest publicou um relato sobre a mudança na forma de escrever e manter documentação interna.

## Problema

Segundo o relato, as ferramentas de documentação usadas antes:

- dificultavam propor mudanças e iterar com base em feedback;
- não garantiam que todas as pessoas interessadas revisassem as atualizações;
- deixavam a documentação longe do código, o que prejudicava a descoberta;
- usavam editores visuais (WYSIWYG) que misturavam estilo e conteúdo.

## Abordagem

- Padronização em **Markdown + Git**, com a documentação passando pelo mesmo fluxo de revisão e publicação do código.
- Criação do **PDocs (Pinterest Docs)**, ferramenta interna que percorre os repositórios procurando arquivos `pdocs.yaml`, converte o Markdown indicado em HTML e gera um site central de documentação, com metadados, templates e busca.
- Uma CLI para criar projetos de documentação e visualizar as mudanças localmente.
- Um **conversor de wiki para PDocs**, para migrar o conteúdo que já existia.

## Resultados relatados

- O número de projetos de documentação **cresceu 20% em dois meses**, passando de 140.
- Pesquisas internas indicaram que escrever e navegar na documentação com o PDocs era uma experiência melhor que nas ferramentas de wiki anteriores.

## O que podemos aprender

- A barreira para documentar não era só cultural — era também de **processo e ferramenta**. Quando ficou fácil, mais gente documentou.
- A **migração** do conteúdo antigo fez parte da solução. Sem ela, a ferramenta nova começaria vazia.

## Limitações

- É um relato da própria empresa, não um estudo independente.
- O número mede quantidade de projetos de documentação, não qualidade ou impacto direto (como tempo de onboarding).
- O Pinterest tinha estrutura para construir uma ferramenta interna; times menores provavelmente usariam algo pronto (veja [ferramentas](../docs-as-code/o-que-e-docs-as-code.md#ferramentas-comuns)).

## Fonte original

- [Adopting Docs-as-Code at Pinterest](https://medium.com/pinterest-engineering/adopting-docs-as-code-at-pinterest-4f18ad169c25) — Pinterest Engineering Blog.
- [Docs-as-Code at Pinterest](https://www.infoq.com/news/2025/06/docs-as-code-at-pinterest) — Sergio De Simone, InfoQ, 16 jun. 2025.
