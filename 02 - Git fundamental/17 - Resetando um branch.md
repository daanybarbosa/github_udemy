# Desfazendo/Resetando todas as alterações de uma branch

- Com o comando **git reset** podemos resetar as mudanças feitas; (resetar um estado)
- Geralmente é utilizado com a flag **--hard**;
- Todas as alterações **commitadas** e **também as pendentes** serão excluidas;

```$ git reset --hard <origem/nome_da_branch>```
```$ git reset --hard origin/master``` -> resete forçado e ira limpar todos os arquivos em stage commits 
