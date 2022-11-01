# curso_git_filipe


## [GIT PUSH comandos fundamentais](https://www.atlassian.com/br/git/tutorials/syncing/git-push)

```
 git checkout main
```

```
 git fetch origin main
```

```
 git rebase -i origin/main
```

```
 git push origin main
```

## [Como resolver o erro “xcrun: error: invalid active developer path” no macOS](https://marcoandrei.com/como-resolver-o-erro-xcrun-error-invalid-active-developer-path-no-macos/)

```
 xcode-select --install
```


[Dillinger - Editor de Markdown ](https://dillinger.io/)


## Iniciando um Repositório

 ```
  git init
 ```
 
### Apagando um repositório
```sh 
rm -rf .git 
```


### Configurar o repositorio remoto > 
```sh
 git config - -global user.name “seu nome”
 git config  - - global user.email “seu email”
```
```sh
 git remote add main (remote directory )
```

### Listando Arquivos Modificados
```sh
git status
```

### Listando Branches

 ```sh
  git branch
 ```
 
 ```sh
 git branch -a (lista as branchs em local remoto)
 ```

### Indo para outra branch
Para mudar para uma outra branch basta usar o comando checkout, passando o nome da branch.

```sh
$ git checkout minha-branch
```

### E você adicionar -b, uma nova branch será criada.
```sh
$ git checkout -b minha-nova-branch
```

### Excluindo branches
Para excluir uma branch local basta executar o comando branch com -d ou -D, passando o nome da branch que você quer apagar.

```sh
git branch -d nome-da-branch
git branch -D nome-da-branch
```

##### A opção -d é mais segura, pois ela só apaga a branch se você já tiver feito merge ou enviado as alterações para seu repositório remoto, evitando perda de código.
A opção -D ignora o estado da sua branch, forçando a sua remoção.
Esse comando apaga apenas a branch local, não removendo branches remotas.


### Renomeando branches
Para renomear a sua atual branch local, execute o comando branch com a opção -m, passando o novo nome.

```sh
git branch -m novo-nome-da-branch
```

### Se você estiver em uma branch e quiser renomear outra, você deve passar primeiro o nome atual da branch que quer renomear:
```sh
git branch -m nome-atual novo-nome


