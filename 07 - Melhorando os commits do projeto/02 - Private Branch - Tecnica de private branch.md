# Branches com commits ruins

- Há uma solução chamada **private branches**;
- Onde criamos branches que **não são compartilhados no repositorio**, então podemos colocar qualquer commit;
- É um repositorio apenas para ser trabalhado e quando a funcionalidade estiver pronta, realizar um unico commit.
- Ao fim da solução do problema podemos fazer um **rebase**;
- O comando será: **git rebase <atual> <funcionalidade> -i**;
- Escolhemos os branches para excluir(**squash**), renomear com (**reword**) ou permanecer (**pick**) os commits;

```$ git rebase <branch_atual> <branch_funcionalidade> -i``` -> colocar no branch atual as funcionalidades do branc_funcionalidade apenas considerando os commits bons
```$ git rebase func_a private_func_a -i``` - exemplo


```$ git branch``` 
```$ git checkout -b func_a```  -> nova funcionalidade 
```$ git branch``` 
```$ git checkout -b private_func_a``` -> outra nova funcionalidade
```$ git commit -a -m "criando arquivo da funcao"``` -> commit bom
```$ git commit -a -m "."``` -> commit ruim
```$ git commit -a -m "parei aqui"``` -> commit ruim
```$ git commit -a -m "falta so aquela funcao"``` -> commit ruim
```$ git commit -a -m "adicionada a funcao de criar produto"``` -> commit bom

```$ git checkout -b func_a```  -> trazer as funcoes para esse branch
```$ git rebase func_a private_func_a -i```


- Colocar no branch atual as funcionalidades do branc_funcionalidade apenas considerando os commits bons
    pick -> levar todos os commits 
    - para modificar os commits, aperte o "i" (insert)
    - para deletar ou renomear os commits ruins, substitui o "pick" por "squash" ou "reword"
    - para fechar "esc"
    - para salvar o rebase ":x!"

**pick** <id_commit> criando arquivo da funcao
**squash** <id_commit> .
**reword** <id_commit> parei aqui
**squash** <id_commit> falta so aquela funcao
**pick** <id_commit> adicionada a funcao de criar produto
