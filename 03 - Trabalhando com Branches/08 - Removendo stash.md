# Removendo a stash

- Para limpar totalmente as stash de uma branch podemos utilizar o comando **git stash clear**;
- Caso seja necessário deletar uma stash especifica podemos utilizar **git stash drop <identificador_stash>**;

```$ git stash clear``` -> apagar todas as stash do branch atual serão deletadas
```$ git stash drop <identificador_stash>``` -> deletar uma stash especifica

**Exemplo**
```$ git stash list``` -> listar todas as stash
```$ git stash drop 5``` -> deletar a stash 5
```$ git stash clear``` -> deletar todas as stash
