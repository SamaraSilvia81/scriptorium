<picture>
  <source media="(prefers-color-scheme: light)" srcset="_assets/banners/banner-topo-claro.webp">
  <img src="_assets/banners/banner-topo.webp" alt="Scriptorium — onde se escreve o que o código não diz" width="100%">
</picture>

# Padrão do acervo

Como o Scriptorium se organiza: pastas, nomes de arquivo, metadados, imagens e o que pode ou não entrar. O padrão existe para que qualquer documento seja fácil de encontrar, citar e manter — inclusive daqui a dois anos.

> Este padrão é uma adaptação de um sistema que uso para documentos de trabalho, ajustado para um repositório Git público.

## Sumário

1. [Pastas](#1-pastas)
2. [Nomes de arquivo](#2-nomes-de-arquivo)
3. [Tipos de documento](#3-tipos-de-documento)
4. [Metadados](#4-metadados)
5. [Status](#5-status)
6. [Imagens e banners](#6-imagens-e-banners)
7. [O que não entra](#7-o-que-não-entra)
8. [Como adicionar um documento](#8-como-adicionar-um-documento)
9. [Por que não há revisão no nome](#9-por-que-não-há-revisão-no-nome)

## 1. Pastas

Formato `NN-nome`, em minúsculas. O número define a ordem de leitura no GitHub e **não é reaproveitado**: se uma pasta for removida, o número dela fica vago.

| Pasta | Conteúdo |
|---|---|
| `01-fundamentos/` | Conceitos e princípios: por que documentar, para quem, como organizar |
| `02-docs-as-code/` | Documentação com práticas de desenvolvimento: versionamento, revisão, automação |
| `03-na-pratica/` | Guias e checklists para aplicar em projetos |
| `04-casos/` | Experiências públicas de organizações, sempre com fonte |
| `90-modelos/` | Modelos para criar documentos novos |
| `_assets/` | Banners, diagramas e o gerador de banners |

A faixa `90+` é reservada para pastas de apoio. Pastas novas de conteúdo entram com o próximo número livre (`05-`, `06-`...) **quando houver o primeiro documento** — pasta vazia não entra.

## 2. Nomes de arquivo

```
TIPO-NNN-descricao.md
```

| Parte | Exemplo | Regra |
|---|---|---|
| Tipo | `NOT` | Sigla de três letras (seção 3) |
| Número | `001` | Sequência por tipo, no acervo inteiro. Não é reaproveitado |
| Descrição | `por-que-documentar` | Minúsculas, hífen, sem acento |

O código (`NOT-001`) é a identidade do documento. Ele aparece no título, na tabela de metadados e é a forma de citar o texto em outros documentos ou posts.

Cada pasta tem um `README.md` que lista o que há nela. Esse arquivo não leva código.

## 3. Tipos de documento

| Sigla | Tipo | Para quê | Modelo |
|---|---|---|---|
| `NOT` | Nota de estudo | Estudar um conceito, prática ou ferramenta | [`MOD-001`](90-modelos/MOD-001-nota-de-estudo.md) |
| `GUI` | Guia prático | Algo para aplicar: guia, checklist, receita | [`MOD-003`](90-modelos/MOD-003-guia-pratico.md) |
| `CAS` | Registro de caso | Experiência pública de uma organização | [`MOD-002`](90-modelos/MOD-002-registro-de-caso.md) |
| `MOD` | Modelo | Estrutura para criar documentos novos | — |

## 4. Metadados

Todo documento começa com o banner da seção, o título com o código e uma tabela de metadados:

| Campo | Obrigatório | Conteúdo |
|---|---|---|
| Código | Sim | `TIPO-NNN` |
| Tipo | Sim | Nota de estudo, guia prático, registro de caso |
| Status | Sim | Ver seção 5 |
| Criado em | Sim | DD/MM/AAAA |
| Última atualização | Sim | DD/MM/AAAA e link para o histórico do arquivo no GitHub |
| Relacionados | Não | Códigos de outros documentos, com link |
| Organização / Fonte | Só em `CAS` | Quem e que tipo de fonte |

Logo depois, uma linha de destaque (`>`) com a **pergunta principal** (notas), o **objetivo** (guias) ou o **resumo em uma frase** (casos), seguida do sumário numerado.

## 5. Status

| Status | Significado |
|---|---|
| Rascunho | Em escrita. Pode estar incompleto |
| Em revisão | Completo, sendo conferido (fontes, links, texto) |
| Publicado | Revisado e listado na tabela do README |
| Em apuração | Caso cuja fonte ainda não foi conferida. Não entra na tabela até mudar de status |
| Arquivado | Mantido por histórico, mas desatualizado. O motivo vai no topo do documento |

## 6. Imagens e banners

- Ficam em `_assets/banners/` e `_assets/diagramas/`.
- Formato **WebP**, para manter o repositório leve.
- Toda imagem tem duas versões: `nome.webp` (tema escuro, padrão) e `nome-claro.webp` (tema claro). No Markdown, usam `<picture>` para o GitHub escolher conforme o tema de quem lê.
- Diagramas seguem a identidade visual (fundo void, phosphor e ember, Space Grotesk, Inter e JetBrains Mono) e trazem a fonte no rodapé.
- Toda imagem tem `alt` descrevendo o conteúdo, não só o título.
- Banners novos saem do [`gerador-banners-scriptorium.html`](_assets/gerador-banners-scriptorium.html).

## 7. O que não entra

Este repositório é público. Não entra:

- **Material de trabalho ou de cliente** — documentos, prints, atas, nomes de projetos internos, mesmo que anonimizados de forma parcial.
- **Informação protegida por termo de sigilo** ou que alguém compartilhou em confiança.
- **Dados da pesquisa de mestrado ainda não publicados.** Só entra o que já é público, e com a referência.
- **Casos sem fonte pública verificável.** Se não dá para linkar, não é caso — no máximo, opinião identificada numa nota.
- **Texto de terceiros copiado.** Resuma com suas palavras e cite; trechos curtos entre aspas, com fonte.

Na dúvida, não publique.

## 8. Como adicionar um documento

1. Escolha o tipo e copie o modelo correspondente (seção 3).
2. Dê o próximo número livre do tipo — confira na tabela do [README](README.md#-documentos).
3. Escreva com status **Rascunho**.
4. Antes de publicar, siga o checklist do modelo.
5. Mude o status para **Publicado**, adicione a linha na tabela do README e no `README.md` da pasta.
6. Commit em inglês, por exemplo: `git commit -m "docs: add NOT-004 on architecture decision records"`

## 9. Por que não há revisão no nome

No sistema original, o nome do arquivo leva a revisão (`R00`, `R01`) e versões antigas vão para uma pasta de obsoletos. Aqui isso não existe porque **o Git já guarda todas as versões**: o link de histórico na tabela de metadados mostra cada mudança, quando foi feita e por quê. Duplicar versões em arquivos seria justamente o contrário do que [docs-as-code](02-docs-as-code/NOT-003-o-que-e-docs-as-code.md) propõe.

<picture>
  <source media="(prefers-color-scheme: light)" srcset="_assets/banners/banner-rodape-claro.webp">
  <img src="_assets/banners/banner-rodape.webp" alt="Scriptorium · rodapé" width="100%">
</picture>
