# Git Customized Commands

[![CI](https://github.com/jonathanmdr/GitCustomizedCommands/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/jonathanmdr/GitCustomizedCommands/actions/workflows/ci.yml)

Criando comandos customizados `git` para facilitar e simplificar as atividades diárias de quem gosta de trabalhar com `git` via terminal.

### Como funciona:

São simples shell scripts que executam os comandos `git` internamente, reduzindo a verbosidade dos comandos de forma bem significativa.

> :warning: Os scripts foram testados em distribuições Linux baseadas em Ubuntu e MacOS.

É recomendado que os scripts sejam armazenados no diretório `/usr/local/bin`.
> Os scripts podem ser armazenados em outro diretório `/bin`.

### Sobre os scripts:

Script | Descrição
--|--|
`git-create-branch` | Cria um novo `branch` local baseado no `branch` atual, envia para o repositório remoto e faz um `checkout` no novo branch.
`git-purge-branchs` | Deleta todos os `branchs` que já foram mergeados no `branch` principal do repositório, atualmente são considerados `branchs` principais os que estão identificatos com o nome `main` ou `master`.
`git-log-graph` | Exibe toda a árvore de `branchs` com detalhamento dos `commits`, `users` e `merges` que foram realizados no repositório.

#### Como executar:
```sh
# Criando um novo branch e aplicando checkout
git create-branch <nome-do-branch-que-deseja-criar>

# Deletando os branchs que já foram mergeados no branch principal
git purge-branchs

# Exibindo a árvore do repositório
git log-graph
```
