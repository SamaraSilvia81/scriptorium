# Por que documentar — e por que a gente sempre deixa pra depois

> **Status:** publicado
> **Tipo:** nota de estudo (com opinião identificada)

## A cena

Você encontra um repositório que parece resolver exatamente o seu problema. O código é bom. O README tem três linhas. A instalação não funciona do jeito descrito, e não existe explicação de por que o projeto foi organizado daquele jeito.

Você fecha a aba e procura outra coisa.

O projeto podia ser excelente. Você nunca vai saber.

## O problema não é falta de vontade

Quase ninguém discorda de que documentação importa. Mesmo assim, ela vive no fim da fila. Alguns motivos aparecem com frequência:

- **Ela não quebra nada quando falta.** O build passa, os testes passam, o deploy acontece.
- **O custo aparece em outro lugar.** Quem paga é quem chega depois: a pessoa nova no time, quem vai dar manutenção, quem tenta usar a API.
- **Ela parece separada do trabalho "de verdade".** Quando a documentação mora longe do código, atualizá-la vira uma tarefa extra — e tarefa extra é a primeira a ser cortada.

## Documentação ausente também é dívida

*(Opinião, conectada aos meus estudos em engenharia de software.)*

Dívida técnica costuma ser associada a código: atalhos, gambiarras, decisões que cobram juros depois. Mas a falta de documentação funciona do mesmo jeito. A decisão de "não documentar agora" economiza tempo hoje e cobra depois — em perguntas repetidas, em onboarding lento, em conhecimento que vai embora quando alguém sai do time.

A diferença é que essa dívida é **invisível**: nenhuma ferramenta de análise estática vai apontar que a decisão mais importante do sistema nunca foi escrita em lugar nenhum.

Esse tema vai ganhar uma nota própria aqui no repositório.

## O que ajuda na prática

Não existe receita única, mas algumas ideias aparecem em vários contextos:

1. **Saber para quem se escreve.** Quem está aprendendo precisa de algo diferente de quem só quer consultar um parâmetro. → [Diátaxis](diataxis.md)
2. **Deixar a documentação perto do código.** Se ela passa pelo mesmo fluxo de revisão, ela tem mais chance de acompanhar as mudanças. → [Docs-as-code](../docs-as-code/o-que-e-docs-as-code.md)
3. **Começar pelo mínimo útil.** Um README que explica o que é, como rodar e onde procurar ajuda já resolve boa parte do problema. → [Checklist de README](../na-pratica/checklist-readme.md)

## E existem casos reais

Quando o Pinterest passou a tratar documentação com o mesmo fluxo do código, o número de projetos de documentação cresceu 20% em dois meses. → [Caso completo](../casos-e-referencias/pinterest-docs-as-code.md)

## Referências

- [Adopting Docs-as-Code at Pinterest](https://medium.com/pinterest-engineering/adopting-docs-as-code-at-pinterest-4f18ad169c25) — Pinterest Engineering.
- [Diátaxis](https://diataxis.fr/) — Daniele Procida.
- [Docs as Code](https://www.writethedocs.org/guide/docs-as-code/) — Write the Docs.
