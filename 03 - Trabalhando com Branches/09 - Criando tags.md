# Utilizando tags

- Podemos criar tags nos branches por meio do comando **git tag -a <nome> -m "<msg>"**;
- A tag é diferente do stash, serve como um **checkpoint de um branch**;
- É utilizada para demarcar estágios do desenvolvimento de algum recurso;

```$ git tag``` -> lista das tags
```$ git tag -a <nome> -m "<msg>"```
```$ git tag -a v1.0 -m "Primeira versão"``` -> exemplo


**Exemplo**
```$ git tag -a v1.0 -m "Primeira versão"``` -> primeira tag criada
```$ git tag``` - listar as tags existentes
```$ git status``` -> verificar as alterações do arquivo
```$ git commit -a -m "Enviando alteracoes``` -> enviando commit das alteracoes
```$ git tag -a v2.0 -m "Segunda versão"``` -> segunda tag criada

