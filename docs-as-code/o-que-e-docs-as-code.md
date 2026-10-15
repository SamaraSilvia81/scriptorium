# O que é docs-as-code

> **Status:** publicado
> **Tipo:** nota de estudo

## Pergunta principal

Se a documentação desatualiza tão fácil, e se ela seguisse o mesmo caminho do código?

## A ideia

*Docs-as-code* é tratar documentação com as mesmas ferramentas e o mesmo fluxo usados para desenvolver software:

| No código | Na documentação |
|:---|:---|
| Arquivos de texto versionados | Markdown, MDX, AsciiDoc no repositório |
| Git | Histórico de mudanças da documentação |
| Pull request e revisão | Revisão de texto junto com a mudança de código |
| CI/CD | Build e publicação automática do site de docs |
| Testes e lint | Verificação de links quebrados, ortografia, estilo |

## Por que isso ajuda

- **A documentação muda junto com o código.** Se uma PR altera um comportamento, a mesma PR pode atualizar a doc — e a revisão pega quando isso não acontece.
- **Quem escreve código já sabe usar as ferramentas.** Não precisa aprender outro sistema nem pedir acesso a uma wiki separada.
- **Fica rastreável.** Dá para saber quando, por que e por quem uma informação mudou.

## Ferramentas comuns

Algumas opções para gerar sites de documentação a partir de Markdown:

- [Docusaurus](https://docusaurus.io/) — React, comum em projetos open source.
- [Astro Starlight](https://starlight.astro.build/) — Astro, leve e com boa experiência padrão.
- [MkDocs](https://www.mkdocs.org/) / [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) — Python, muito usado em documentação técnica.
- [VitePress](https://vitepress.dev/) — Vue/Vite.

E para checar qualidade do texto: [Vale](https://vale.sh/) (lint de estilo) e verificadores de links no CI.

## Limitações

- Docs-as-code melhora o **processo**, não garante a **qualidade** do texto. Uma doc ruim versionada continua ruim.
- Para pessoas que não usam Git no dia a dia (produto, suporte, design), a barreira de entrada pode aumentar.
- Exige combinar no time que mudança sem doc não está pronta.

## Na prática

O [caso do Pinterest](../casos-e-referencias/pinterest-docs-as-code.md) mostra uma empresa grande migrando de wiki para docs-as-code.

## Referências

- [Docs as Code](https://www.writethedocs.org/guide/docs-as-code/) — Write the Docs.
- [Adopting Docs-as-Code at Pinterest](https://medium.com/pinterest-engineering/adopting-docs-as-code-at-pinterest-4f18ad169c25) — Pinterest Engineering.
