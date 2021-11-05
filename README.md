# Git Customized Commands

Criando comandos customizados `git` para facilitar e simplificar as atividades diárias de quem gosta de trabalhar com `git` via terminal.

### Como isso funciona:

São simples shell scripts que executam os comandos `git` internamente, reduzindo a verbosidade dos comandos de forma bem significativa.

> :warning: Os scripts foram testados em distribuições Linux baseadas em Ubuntu e MacOS.

É recomendado que os scripts sejam armazenados no diretório `/usr/local/bin` e é preciso garantir que os mesmos já tenham a permissão de execução.
> Os scripts podem ser armazenados em outro diretório `/bin`.

#### Como permitir que o script seja executável:
> :warning: Pode ser preciso utilizar `sudo`.
```sh
chmod +x <nome-do-script>
```

### Sobre os scripts:

Script | Descrição
--|--|
`git-create-branch` | Cria um novo `branch` baseado em um `branch` qualquer e faz um `checkout` para o novo branch criado.
`git-purge-branchs` | Deleta todos os `branchs` que já foram mergeados nos branchs principais identificatos como `main` ou `master`.
`git-log-graph` | Exibe toda a árvore de `branchs` com os `commits` e `merges` que foram realizados.

#### Como executar:
```sh
# Criando um novo branch e aplicando checkout
git create-branch <nome-do-branch-que-deseja-criar>

# Deletando os branchs que já foram mergeados no branch principal
git purge-branchs

# Exibindo a árvore do repositório
git log-graph
```
