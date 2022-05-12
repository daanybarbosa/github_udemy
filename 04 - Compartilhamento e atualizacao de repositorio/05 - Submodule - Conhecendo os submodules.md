# Trabalhando com submódulos

- Submódulo é a maneira que temos de possuir **dois ou mais projetos em um só repositorio**;
- Podemos adicionar uma dependência ao nosso projeto atual, porém mantendo suas estruturas separadas;
- Para adicionar o submódulo utilizamos o comando **git submodule add <link_do_repo>**;
- Para verificar os submódulos o comando é **git submodule**;
- Cria o arquivo **.gitmodules** usado para controlar os submodulos desse projeto;

```$ git submodule``` -> verificar os submodulos existentes
```$ git submodule add <link_do_repo> <local_repositorio>``` -> adicionar um submodulo 
```$ git submodule add https://github submodulo``` -> adicionar um submodulo (cria uma pasta chamada submodulo no repositorio atual)

**Exemplo**
- Criar um novo repositorio no GitHub.
```$ cd .\submodulo\``` -> acessar a pasta submodulo
```$ git pull``` -> atualiza o submodulo
