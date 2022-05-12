# Exibindo informações

- O comando **git show** nos dá diversas informações uteis;
- Ele nos dá as informações do **branch atual e também seus commits**;
- As **modificações de arquivos** entre cada commit também são exibidas;
- Podemos exibir as informações de tags também com: **git show <tag>**;

```$ git show``` -> exibi informações bem detalhadas do branch atual e dos seus commits
```$ git show <tag>``` -> exibi informações bem detalhadas de uma tag
```$ git show v1.0``` -> visualizar os detalhes dessa tag v1.0

**Exemplo**
```$ git branch```
```$ git fetch -a```
```$ git show``` -> mostrar os detalhes desse branch 
```$ git chechout -b "testando_show"``` -> criando um novo branch
```$ git show``` -> detalhes do novo branch
```$ git status``` -> nao tem nenhuma modificação nesse branch 
```$ git branch``` -> visualizar o branch atual -> testando_show
```$ git add .``` -> adicionar novos arquivos a esse branch
```$ git commit -a -m "enviando alteracoes"``` -> adicionar novos arquivos a esse branch
```$ git push``` -> enviando as alterações
```$ git push --set-upstream origin testando_show``` -> enviando alterações
```$ git show``` -> detalhes/modificações do novo branch
```$ git tag``` -> visualizar as tags presentes
```$ git tag -a v5.0 -m "Versão 5"``` - criar uma nova tag v5.0
```$ git show v4.0``` -> visualizar os detalhes dessa tag v4.0
```$ git show v5.0``` -> visualizar os detalhes dessa tag v5.0
```$ git show v1.0``` -> visualizar os detalhes dessa tag v1.0