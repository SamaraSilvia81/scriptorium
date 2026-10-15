# Checklist de README

> **Status:** publicado
> **Tipo:** guia prático

Um checklist para revisar o README de um projeto. Nem todo item se aplica a todo projeto — use como ponto de partida, não como regra.

## O essencial

Se o README só tiver isso, já resolve boa parte do problema.

- [ ] **O que é** — uma ou duas frases explicando o projeto para quem nunca ouviu falar dele.
- [ ] **Para que serve** — qual problema resolve ou para quem foi feito.
- [ ] **Como rodar** — pré-requisitos e comandos para instalar e executar, testados de verdade.
- [ ] **Como usar** — um exemplo mínimo funcionando.
- [ ] **Status** — ativo, em construção, arquivado?

## Para projetos que vão receber outras pessoas

- [ ] **Estrutura de pastas** — o que fica onde, em poucas linhas.
- [ ] **Como contribuir** — ou link para o `CONTRIBUTING.md`.
- [ ] **Licença** — sem licença, legalmente ninguém pode reutilizar o código.
- [ ] **Onde pedir ajuda** — issues, discussões, contato.

## Para projetos maiores

- [ ] **Links para documentação completa** — o README vira porta de entrada, não o manual inteiro. (Veja [Diátaxis](../fundamentos/diataxis.md).)
- [ ] **Decisões importantes** — por que a arquitetura é assim, ou link para os ADRs.
- [ ] **Variáveis de ambiente e configuração** — o que precisa existir para o projeto funcionar.

## Sinais de alerta

- O comando de instalação não funciona numa máquina limpa.
- O README descreve uma versão antiga do projeto.
- Tem badge, logo e emoji, mas não diz o que o projeto faz.
- Tudo está num bloco único, sem títulos.

## Teste rápido

Peça para alguém que nunca viu o projeto ler o README e tentar rodar. Onde a pessoa travar, falta documentação.

## Referências

- [Make a README](https://www.makeareadme.com/) — guia e modelo comunitário.
- [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes) — GitHub Docs.
