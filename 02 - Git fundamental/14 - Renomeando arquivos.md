# Renomeando arquivos

- Com o comando **git mv** podemos renomear um arquivo;
- O mesmo também pode ser **movido para outra pasta**;
- E isso fará comque este novo **arquivo seja monitorado pelo git**;
- O arquivo anterior é **excluido**;

```$ git mv <nome_do_arquivo> <pasta_de_destino>``` -> mover o arquivo
```$ git mv rodape.css css/rodape.css```
```$ git mv <pasta/arquivo_atual> <pasta/novo_nome_do_arquivo>``` -> renomear o arquivo
```$ git mv css/bannerinicia.css css/banner_inicial.css``` 


**Exemplo para mover o arquivo**
```$ git mv rodape.css css/rodape.css```  
```$ git status``` 
```$ git commit -a -m "Colocando o arquivo css na pasta certa"``` 
```$ git push``` 

**Exemplo para renomear o arquivo**
```$ git mv css/bannerinicia.css css/banner_inicial.css```  
```$ git status``` 
```$ git commit -a -m "Renomeando arquivo"``` 
```$ git push``` 