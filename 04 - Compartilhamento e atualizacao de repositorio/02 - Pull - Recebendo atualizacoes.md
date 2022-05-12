# Recebendo alterações

- O comando **git pull** serve para recebemos atualizações do repositorio remoto;
- Cada branch pode ser atualizado com o git pull, inclusive a main;
- Utilizamos para atualizar a master do repo como também quando trabalhamos em conjunto e queremos receber as atualizações de um dev;

```$ git pull``` -> recebemos atualizações do repositorio remoto.


**Exemplo**
```$ git checkout main``` -> entrar no repositorio main
```$ git pull``` -> atualizar o repositorio

```$ git checkout -b "adicionar_css_home"``` -> -> muda e cria uma nova branch
```$ git commit -a -m "enviando css"``` -> commit
```$ git push``` -> enviando as mudanças (erro - ele não está no repositorio novo ainda)
```$ git push --set-upstream origin adicionar_css_home``` -> enviando as mudanças 

**Atualizar a master/main**
```$ git branch``` -> conferindo se está na master/main
```$ git pull``` -> atualizar o repositorio
```$ git merge adicionar_css_home``` -> erro - a branch está na origin
```$ git merge origin/adicionar_css_home``` -> unir as mudanças da branch "adicionar_css_home" com o main
```$ git status```
```$ git push``` -> atualizar a main no repositorio tbm 

**Branch - Nova tarefa**
```$ git branch``` -> branch atual
```$ git checkout main``` -> ir para o branch main (repositorio mais atualizado)
```$ git pull``` -> atualizar o repositorio
```$ git checkout -b "nova_tarefa"``` -> atualizar o repositorio
```$ git branch```