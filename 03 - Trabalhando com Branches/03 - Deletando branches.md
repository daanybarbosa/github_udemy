# Deletando branches

- Podemos deletar um branch com a flag **-d** ou **--delete**;
- **Não é comum deletar um branch**, normalmente guardamos o historico do trabalho;
- Geralmente se usa o delete quando o branch foi criado errado;

```$ git branch -d <nome_do_branch>``` -> deletando um branch
```$ git branch --delete <nome_do_branch>``` -> outra forma de deletar um branch
```$ git branch -d primeiro_branch``` -> exemplo

```$ git branch``` -> lista todos os branches do projeto
```$ git branch -d segundo_branch``` -> deletando o segundo branch
```$ git branch --delete primeiro_branch``` -> deletando o primeiro branch