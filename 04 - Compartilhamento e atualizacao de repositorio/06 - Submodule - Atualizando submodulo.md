# Atualizando submódulo

- Para atualizar um submódulo primeiro devemos **commitar as mudanças**;
- E para enviar para o repo do submódulo utilizamos **git push --recurse-submodule=on-demand**;
- Este fluxo fará a atualização apenas do submódulo;

```$ git push --recurse-submodules=on-demand```


**Exemplo**
```$ git status``` -> verificar se houve alterações na pasta do submodulo;
```$ git add .``` -> adicionar algum arquivo alterado ao submodulo
```$ git commit -a -m "enviando arquivo ao submodulo"``` -> commit das mudanças ao submódulo
```$ git push --recurse-submodules=on-demand``` -> enviar o arquivo ao submodulo


