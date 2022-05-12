# Desfazendo alterações

- O arquivo modificado pode ser **retornado ao estado original**;
- O comando utilizado é o **git checkout**;
- Após a utilização do mesmo o arquivo sai do staging;
- Caso seja feia uma próxima alteração, ele entra em staging novamente;

```$ git checkout <pasta/nome_do_arquivo>``` -> ira resertar todas as moficações do arquivo e ira deixar igual que está salvo no repositorio.
```$ git checkout css/styles.css``` 