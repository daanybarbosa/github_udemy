# Verificando e alterando tags

- Podemos verificar uma tag com o comando **git show <nome>**;
- Podemos trocar de tags com o comando **git checkout <nome>**;
- Desta maneira podemos retroceder ou avançar em checkpoints de um branch;
- Criar um ponto de recuperação no código 

```$ git show <nome_da_tag>```
```$ git show v1.0``` -> visualizar os detalhes da tag v1.0
```$ git checkout <nome_da_tag>``` -> Troca de tags
```$ git chechout v1.0``` -> Voltar para a tag v1.0


**Exemplo**
```$ git tag``` -> listar as tags
```$ git show v1.0``` -> visualizar os detalhes da tag v1.0
```$ git show v2.0``` -> visualizar os detalhes da tag v2.0
```$ git tag -a v3.0 -m "Terceira versao"``` -> criar a tag v3.0
```$ git show v3.0``` -> visualizar os detalhes da tag v3.0
```$ git commit -a -m "Enviando alt``` -> visualizar os detalhes da tag v2.0
```$ git tag -a v4.0 -m "Quarta versao"``` -> criar a tag v4.0
```$ git show v4.0``` -> visualizar os detalhes da tag v4.0

```$ git chechout v1.0``` -> Voltar para a tag v1.0