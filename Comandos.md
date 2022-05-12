# Comandos Fundamentais

```$ git --version``` -> confirmar a instalação e verificar a versão do git.
```$ git init``` - criar um repositório (é apenas usado uma vez ao inicializar um novo repositório);
```$ git status``` - verificar o status/mudanças do projeto

**Adicionando arquivos ao projeto**
```$ git add <arquivo>``` -> comando
```$ git add index.html``` -> adicionar o arquivo index.html
```$ git add .``` -> adicionar todos os arquivos

**Salvando alterações**
```$ git commit a.txt -m "Estou enviando o arquivo de texto"``` -> commitar o arquivo a.txt com uma mensagem
```$ git commit -a -m "Enviando a funcionalidade X"``` -> commitar todos os arquivos com uma mensagem

***Enviar o código ao repositorio**
```$ git push``` -> enviar o codigo ao repositorio remoto (github)

**Recebendo as mudanças**
```$ git pull``` -> sincronizar o codigo atual com o existente na máquina.

**Clonar o repositorio**
```$ git clone <url_repositorio> . ``` - clonar o repositorio na pasta atual

**Removendo arquivos do repositorio**
```$ git rm <arquivo>``` -> Removendo arquivos do repositorio
```$ git rm c.txt```

**Histórico de alterações**
```$ git log``` -> ira visualizar as alterações/modificacoes que foram feitas nesse projeto/repositorio

**Renomeando arquivos ou mover para outra pasta**
```$ git mv <nome_do_arquivo> <pasta_de_destino>``` -> mover o arquivo
```$ git mv rodape.css css/rodape.css```
```$ git mv <pasta/arquivo_atual> <pasta/novo_nome_do_arquivo>``` -> renomear o arquivo
```$ git mv css/bannerinicia.css css/banner_inicial.css``` 

**Desfazendo alterações**
```$ git checkout <pasta/nome_do_arquivo>``` -> ira resertar todas as moficações do arquivo e ira deixar igual que está salvo no repositorio.
```$ git checkout css/styles.css``` 

**Desfazendo/Resetando todas as alterações de uma branch**
```$ git reset --hard <origem/nome_da_branch>```
```$ git reset --hard origin/master``` -> resete forçado e ira limpar todos os arquivos em stage commits 

**Criando e visualizando os branches**
```$ git branch``` -> lista todas as branches disponiveis no projeto
```$ git branch <nome>``` -> criar uma nova branch
```$ git branch primeiro_branch``` -> exemplo

**Deletando branches**
```$ git branch -d <nome_do_branch>``` -> deletando um branch
```$ git branch --delete <nome_do_branch>``` -> outra forma de deletar um branch
```$ git branch -d primeiro_branch``` -> exemplo

**Mudando de branch**
```$ git checkout <nome_da_branch>``` -> mudar para essa branch
```$ git checkout -b <nome_da_nova_branch>``` -> muda e cria uma nova branch

```$ git branch``` -> lista as branches
```$ git checkout algum_nome``` -> mudar para essa branch
```$ git checkout main``` -> voltar para a branch main
```$ git checkout -b teste_criacao_branch``` -> muda e cria uma nova branch

**Unindo branches**
```$ git merge <nome_da_branch>```

Exemplo
```$ git branch```
```$ git checkout teste_criacao_2``` -> quer unir essa branch com a main
```$ git checkout main``` -> mudar para a branch main 
```$ git merge teste_criacao_2``` -> unindo o teste_criacao_2 com a main
```$ git push``` -> atualizar a main no github

**Stash**
```$ git stash``` -> o codigo será refeito, será salvo em algum lugar as alterações e o código será resetado de acordo com o repositorio.

**Recuperando stash**
```$ git stash list``` -> lista as stash criadas
```$ git stash apply <identificador_stash>``` -> aplicando uma stash ao branch
```$ git stash apply 0``` -> exemplo - recuperando tudo presente no stash 0
```$ git stash show -p <identificador_stash>``` -> mostra as alterações/modificações da stash
```$ git stash show -p 0``` -> exemplo

**Removendo stash**
```$ git stash clear``` -> apagar todas as stash do branch atual serão deletadas
```$ git stash drop <identificador_stash>``` -> deletar uma stash especifica
```$ git stash drop 5``` -> exemplo - deletar a stash 5

**Utilizando tags**
```$ git tag``` -> lista das tags
```$ git tag -a <nome> -m "<msg>"```
```$ git tag -a v1.0 -m "Primeira versão"``` -> exemplo

**Verificando e alterando tags**
```$ git show <nome_da_tag>```
```$ git show v1.0``` -> visualizar os detalhes da tag v1.0
```$ git checkout <nome_da_tag>``` -> Troca de tags
```$ git chechout v1.0``` -> Voltar para a tag v1.0

**Enviando tags ao repositorio**
```$ git push origin <nome_da_tag>``` -> enviar a tag para o repositório de código
```$ git push origin v2.0``` -> exemplo - enviar a tag v2.0 para o repositorio
```$ git push origin --tags``` -> enviar todas as tags 

**Encontrando branches**
```$ git fetch``` -> atualiza todas as branches e as tags 
```$ git fetch -a``` -> atualizar todas as branches remotas

**Utilizando o remote**
```$ git remote``` -> adicionar um repo para trackear ou remover
```$ git remote add origin <link_do_repositorio>``` -> adicionar um novo repositorio
```$ git remote -v``` -> visualizar as origens (fetch - receber e push - enviar)
```$ git remote rm origin```-> remover o repositorio

**Trabalhando com submodule**
```$ git submodule``` -> verificar os submodulos existentes
```$ git submodule add <link_do_repo> <local_repositorio>``` -> adicionar um submodulo 
```$ git submodule add https://github submodulo``` -> adicionar um submodulo (cria uma pasta chamada submodulo no repositorio atual)

- Cria o arquivo **.gitmodules** usado para controlar os submodulos desse projeto;

**Atualizando submódulo**
```$ git push --recurse-submodules=on-demand```

Exemplo
```$ git status``` -> verificar se houve alterações na pasta do submodulo;
```$ git add .``` -> adicionar algum arquivo alterado ao submodulo
```$ git commit -a -m "enviando arquivo ao submodulo"``` -> commit das mudanças ao submódulo
```$ git push --recurse-submodules=on-demand``` -> enviar o arquivo ao submodulo

**Exibindo informações**
```$ git show``` -> exibi informações bem detalhadas do branch atual e dos seus commits
```$ git show <tag>``` -> exibi informações bem detalhadas de uma tag
```$ git show v1.0``` -> visualizar os detalhes dessa tag v1.0

**Exibindo diferenças**
```$ git diff <nome_branch>``` -> exibi as diferenças do branch atual com outro branch ou um branch remoto;
```$ git diff main``` -> exemplo
```$ git diff <arquivo> <arquivo_b>``` -> exibi as diferenças de codigos entre arquivos;
```$ git diff HEAD:<nome_do_arquivo_a> <nome_do_arquivo_b>``` -> 
    HEAD:<nome_do_arquivo_a> (arquivo presente no branch remoto), 
    <nome_do_arquivo_b> (arquivo presente no branch atual) - arquivos que estão com o codigo sendo comparados.
```$ git diff HEAD:a.txt a.txt``` -> exemplo

**Log resumido**
```$ git shortlog``` -> log resumido do projeto - ira exibir um panorama completo do projeto, 
    cada commit será unido pelo nome do autor, assim, podemos ver os ultimos commits e quem estava mexendo no código.

**Limpando arquivos untracked**
```$ git clean``` -> limpar arquivos untracked,
    vai verificar e limpar arquivos que não estão sendo trackeados, todos que não foram inclusos no git add;
```$ git clean -f``` -> ira forçar a limpeza

**Otimizando repositorio**
```$ git gc``` -> garbage collector, ele identifica os arquivos que não são mais necessarios e os exclui, tornando o repositorio mais performatico 

**Verificando a integridade dos arquivos**
```$ git fsck``` -> verifica a integridade de arquivos e sua conectividade, evitando corrupções em arquivos.

**Reflog**
```$ git reflog``` -> vai exibir todos os passos no repositorio, como a mudança de um branch, é um comando mais completo do que o git log, ele possui um prazo de expiração que é de 30 dias.

**Comprimindo o repositorio**
```$ git archive --format <formato_da_pasta> --output <nome_da_pasta>.<formato_da_pasta> <branch>``` -> transforma o repo em um arquivo compactado
```$ git archive --format zip --output master_files.zip master``` -> exemplo

----------------------------------------------------------



### …or create a new repository on the command line
- echo "# teste" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin https://github.com/daniele-silva-yssy/teste.git __(adicionando uma origem ao repositorio)__
- git push -u origin main __(enviando da origem para a main)__

### …or push an existing repository from the command line
- git remote add origin https://github.com/daniele-silva-yssy/teste.git
- git branch -M main
- git push -u origin main

### …or import code from another repository
- You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
- __Import Code__


**__os arquivos git estão na pasta oculta .git__**
