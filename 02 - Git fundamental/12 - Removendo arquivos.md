# Removendo arquivos do repositorio

- Os comandos **podem ser deletados da monitoração do** git;
- O comando para deletar é **git rm**;
- Após deletar um arquivo do git ele não terá mais suas atualizações consideradas pelo git;
- Apenas quando for adicionado novamente pelo **git add**;

```$ git rm <arquivo>``` -> Removendo arquivos do repositorio
```$ git rm c.txt```

**Exemplo**
```$ git rm c.txt```
```$ git status``` 
```$ git commit -a -m "Deletando arquivo desnecessario"```
```$ git push```
