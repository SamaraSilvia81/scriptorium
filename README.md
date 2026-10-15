<picture>
  <source media="(prefers-color-scheme: light)" srcset="_assets/banners/banner-topo-claro.webp">
  <img src="_assets/banners/banner-topo.webp" alt="Scriptorium — onde se escreve o que o código não diz" width="100%">
</picture>

<div align="center">

### Estudos, referências e casos reais sobre documentação técnica.

![Status](https://img.shields.io/badge/status-em%20construção-972FFF?style=for-the-badge)
![Formato](https://img.shields.io/badge/formato-docs--as--code-171717?style=for-the-badge)
![Idioma](https://img.shields.io/badge/idioma-pt--BR-171717?style=for-the-badge)

[Fundamentos](01-fundamentos/) · [Docs-as-code](02-docs-as-code/) · [Na prática](03-na-pratica/) · [Casos](04-casos/) · [Modelos](90-modelos/)

[Comece por aqui](01-fundamentos/NOT-001-por-que-documentar.md) · [Padrão do acervo](PADRAO.md) · [Como contribuir](CONTRIBUTING.md)

</div>

---

### $ sobre o projeto

Um *scriptorium* era a sala dos mosteiros medievais onde se escreviam, copiavam e guardavam manuscritos. Este é um scriptorium para **documentação técnica**: um lugar para reunir estudos, referências, guias e casos reais sobre como documentar software — e por que isso importa.

A ideia é explorar como a documentação se conecta ao desenvolvimento: da experiência de quem precisa entender e manter um projeto até decisões de arquitetura, processos de equipe e práticas de *docs-as-code*.

O acervo cresce aos poucos, sem ordem obrigatória. Quando um tema novo aparece, ele entra aqui.

> Não é um manual definitivo. É um caderno de estudo em público.

### $ documentos

| Código | Título | Tipo | Atualizado |
|---|---|---|---|
| [`NOT-001`](01-fundamentos/NOT-001-por-que-documentar.md) | Por que documentar — e por que a gente sempre deixa pra depois | Nota de estudo | 15/10/2026 |
| [`NOT-002`](01-fundamentos/NOT-002-diataxis.md) | Diátaxis: os quatro tipos de documentação | Nota de estudo | 15/10/2026 |
| [`NOT-003`](02-docs-as-code/NOT-003-o-que-e-docs-as-code.md) | O que é docs-as-code | Nota de estudo | 15/10/2026 |
| [`GUI-001`](03-na-pratica/GUI-001-checklist-readme.md) | Checklist de README | Guia prático | 15/10/2026 |
| [`CAS-001`](04-casos/CAS-001-pinterest-docs-as-code.md) | Pinterest e a adoção de docs-as-code | Registro de caso | 15/10/2026 |

**No radar:** documentação como dívida técnica · registros de decisão arquitetural (ADR) · documentação em arquiteturas de microfrontends.

### $ por onde começar

| Se você quer... | Leia |
|---|---|
| Entender por que documentação importa | [`NOT-001`](01-fundamentos/NOT-001-por-que-documentar.md) |
| Organizar a documentação de um projeto | [`NOT-002`](01-fundamentos/NOT-002-diataxis.md) |
| Tratar documentação como parte do código | [`NOT-003`](02-docs-as-code/NOT-003-o-que-e-docs-as-code.md) |
| Melhorar o README do seu projeto agora | [`GUI-001`](03-na-pratica/GUI-001-checklist-readme.md) |
| Ver o que aconteceu numa empresa real | [`CAS-001`](04-casos/CAS-001-pinterest-docs-as-code.md) |

### $ estrutura

```text
scriptorium/
├── 01-fundamentos/      conceitos e princípios          NOT
├── 02-docs-as-code/     práticas, ferramentas e fluxos  NOT
├── 03-na-pratica/       guias e checklists              GUI
├── 04-casos/            experiências públicas           CAS
├── 90-modelos/          modelos de documento            MOD
├── _assets/             banners, diagramas e gerador
├── PADRAO.md            como o acervo se organiza
└── README.md
```

Cada documento tem um código (`NOT-001`, `CAS-001`...), uma tabela de metadados e um link para o próprio histórico. O padrão completo está em [`PADRAO.md`](PADRAO.md).

### $ combinados

- Casos externos sempre vêm com link para a fonte original.
- Opinião e experiência pessoal aparecem identificadas como tal — não como resultado científico.
- Material de trabalho, de cliente ou confidencial não entra (ver [padrão](PADRAO.md#7-o-que-não-entra)).
- A estrutura muda para acompanhar o conteúdo, não o contrário.

### $ participe da conversa

Você já encontrou uma documentação que facilitou muito um projeto — ou a falta dela que tornou tudo mais difícil?

Sugestões de temas, referências e casos públicos são bem-vindos. Veja o [guia de contribuição](CONTRIBUTING.md).

<div align="center">

*Uma nota de cada vez. Uma referência de cada vez.*

Feito por [Samara Silvia](https://github.com/SamaraSilvia81)

</div>

<picture>
  <source media="(prefers-color-scheme: light)" srcset="_assets/banners/banner-rodape-claro.webp">
  <img src="_assets/banners/banner-rodape.webp" alt="Scriptorium · rodapé" width="100%">
</picture>
