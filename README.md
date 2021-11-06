# Git Customized Commands

[![CI](https://github.com/jonathanmdr/GitCustomizedCommands/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/jonathanmdr/GitCustomizedCommands/actions/workflows/ci.yml)

Criando comandos customizados `git` para facilitar e simplificar as atividades diárias de quem gosta de trabalhar com `git` via terminal.

## Como funciona:

São simples shell scripts que executam os comandos `git` internamente, reduzindo a verbosidade dos comandos de forma bem significativa.

> :warning: Os scripts foram testados em MacOS e distribuições Linux baseadas em Ubuntu.

É recomendado que os scripts sejam armazenados no diretório `/usr/local/bin`.
> Os scripts podem ser armazenados em outro diretório `/bin`.

## Sobre os scripts:

Script | Descrição
--|--|
`git-create-branch` | Cria um novo `branch` local baseado no `branch` atual, envia para o repositório remoto e faz um `checkout` no novo branch.
`git-purge-branches` | Deleta todos os `branches` locais que já foram mergeados no repositório remoto, os `branches` ignorados por este script são os que estão identificatos com o nome `main` ou `master`.
`git-log-graph` | Exibe toda a árvore de `branches` com detalhamento dos `commits`, `users` e `merges` que foram realizados no repositório.

### Como executar:

Criando um novo branch:
```sh
git create-branch <nome-do-branch-que-deseja-criar>
```

Deletando branches que já foram mergeados:
```sh
git purge-branches
```

Exibindo a árvore do repositório com detalhes:
```sh
git log-graph
```
