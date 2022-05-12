# Encontrando branches

- Branches novos são criados a todo tempo e o **seu git pode não estar mapeando eles**;
- Com o comando **git fetch** você é atualizado de todos os branches e tags que ainda não estão reconhecidos por você;
- Este comando é util para utilizar o branch de algum outro dev do time, por exemplo;

```$ git fetch``` -> atualiza todas as branches e as tags 
```$ git fetch -a``` -> atualizar todas as branches remotas

**Exemplo**
```$ git chechout -b "funcionalidade_a"```
```$ git commit -a -m "Tarefa pronta"```
```$ git push```
```$ git push --set-upstream origin funcionalidade_a``` -> enviar a funcionalidade_a para o repositorio

```$ git chechout funcionalidade_a``` -> erro - nao existe a branch funcionalidade_a
```$ git fetch -a``` -> atualizar todas as branches remotas - ira mostra que existem uma nova branch "funcionalidade_a" 
```$ git branch``` -> listar os branches existentes 
```$ git chechout funcionalidade_a``` -> consegue ter acesso a essa branch
```$ git chechout main``` -> volta para a branch main
```$ git branch``` -> o novo branch passa a ser nosso
```$ git pull``` -> atualizar o repositorio
