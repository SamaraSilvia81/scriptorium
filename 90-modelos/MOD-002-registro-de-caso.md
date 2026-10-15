<picture>
  <source media="(prefers-color-scheme: light)" srcset="../_assets/banners/banner-topo-claro.webp">
  <img src="../_assets/banners/banner-topo.webp" alt="Scriptorium — onde se escreve o que o código não diz" width="100%">
</picture>

# MOD-002 · Modelo de registro de caso

Use para registrar a experiência de uma organização ou projeto **público** com documentação. Copie o bloco abaixo para `04-casos/CAS-NNN-descricao.md` e siga o [padrão do acervo](../PADRAO.md).

Regra principal: **registre o que a fonte diz, não o que você gostaria que ela dissesse.** Números só entram com fonte e contexto.

````markdown
<picture>
  <source media="(prefers-color-scheme: light)" srcset="../_assets/banners/banner-casos-claro.webp">
  <img src="../_assets/banners/banner-casos.webp" alt="Casos e referências" width="100%">
</picture>

# CAS-NNN · Organização e o tema do caso

| Campo | Valor |
|---|---|
| Código | `CAS-NNN` |
| Tipo | Registro de caso |
| Status | Rascunho |
| Organização | Nome — time, se informado |
| Fonte | Relato da empresa · estudo acadêmico · reportagem · palestra |
| Criado em | DD/MM/AAAA |
| Última atualização | DD/MM/AAAA · [histórico](link) |
| Relacionados | `NOT-...` |

> **Em uma frase:** o que aconteceu e por que importa.

## Sumário

1. [Contexto](#1-contexto)
2. [O problema](#2-o-problema)
3. [A abordagem](#3-a-abordagem)
4. [Resultados relatados](#4-resultados-relatados)
5. [O que podemos aprender](#5-o-que-podemos-aprender)
6. [Limitações do relato](#6-limitações-do-relato)
7. [Fontes](#7-fontes)

## 1. Contexto

Quem publicou, quando, onde e em que situação.

## 2. O problema

O que a fonte relata sobre a situação inicial. Cite trechos curtos quando forem marcantes.

## 3. A abordagem

O que mudou: práticas, ferramentas, processos. Tabela se houver vários componentes.

## 4. Resultados relatados

| Indicador | Valor relatado |
|---|---|
| ... | ... |

## 5. O que podemos aprender

Ideias que parecem úteis além daquele contexto — e quais dependem dele.

## 6. Limitações do relato

Quem mediu? O que não foi medido? O próprio relato reconhece limitações?

## 7. Fontes

- SOBRENOME, Nome. [Título](URL). Veículo, data. Acesso em: DD mmm. AAAA.
````

## Checklist antes de publicar

- [ ] Li a fonte original, não só a notícia sobre ela
- [ ] Todo número da tabela de resultados aparece na fonte
- [ ] O tipo de fonte está claro (relato próprio não é estudo independente)
- [ ] A seção de limitações existe e não está vazia
- [ ] A linha do caso foi adicionada à tabela de documentos do [README](../README.md#-documentos)

<picture>
  <source media="(prefers-color-scheme: light)" srcset="../_assets/banners/banner-rodape-claro.webp">
  <img src="../_assets/banners/banner-rodape.webp" alt="Scriptorium · rodapé" width="100%">
</picture>
