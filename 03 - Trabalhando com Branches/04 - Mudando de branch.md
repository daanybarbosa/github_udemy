# Mudando de branch

- Podemos mudar para outro branch utilizando o comando **git checkout -b <nome>**;
- Este comando também é utilizado para dispensar mudanças de um arquivo;
- Alterando o branch podemos levar alterações que não foram commitadas junto, tome cuidado!;

```$ git checkout <nome_da_branch>``` -> mudar para essa branch
```$ git checkout -b <nome_da_nova_branch>``` -> muda e cria uma nova branch

```$ git branch``` -> lista as branches
```$ git checkout algum_nome``` -> mudar para essa branch
```$ git checkout main``` -> voltar para a branch main
```$ git checkout -b teste_criacao_branch``` -> muda e cria uma nova branch

**Exemplo**
```$ git status```
```$ git commit -a -m "funcionalidade executada"```
```$ git branch```
```$ git checkout main```
```$ git checkout teste_criacao_branch``` -> voltar para o teste_criacao_branch