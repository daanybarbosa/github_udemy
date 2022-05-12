# Unindo branches

- O código de dois branches distintos pode ser unido pelo comando **git merge <nome>**;
- Outro comando para a lista dos **mais utilizados**;
- Normalmente é por meio dele que recebemos as atualizações de outros devs;

```$ git merge <nome>```


**Exemplo**
```$ git branch```
```$ git checkout teste_criacao_2``` -> quer unir essa branch com a main
```$ git checkout main``` -> mudar para a branch main 
```$ git merge teste_criacao_2``` -> unindo o teste_criacao_2 com a main
```$ git push``` -> atualizar a main no github