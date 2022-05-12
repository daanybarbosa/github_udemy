# Recuperando stash

- Podemos verificar as stashs criadas pelo comando **git stash list**;
- E também podemos recuperar a stash com o comando **git stash <identificador_stash>**;
- Desta maneira podemos continuar de onde paramos com os arquivos adicionados a stash;

```$ git stash list``` -> lista as stash criadas
```$ git stash apply <identificador_stash>``` -> aplicando uma stash ao branch
```$ git stash apply 0``` -> exemplo - recuperando tudo presente no stash 0
```$ git stash show -p <identificador_stash>``` -> mostra as alterações/modificações da stash
```$ git stash show -p 0``` -> exemplo 

**Exemplo**
```$ git stash list```
```$ git stash apply 0``` -> recuperando o stash 0
```$ git stash apply 1``` -> error - ira sobreescrever o stash 0
```$ git stash``` -> criar uma nova stash
```$ git stash apply 1``` -> recuperou a stash 1