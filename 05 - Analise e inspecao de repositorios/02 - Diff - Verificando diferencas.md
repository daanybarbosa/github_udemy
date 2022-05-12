# Exibindo diferenças

- O comando **git diff** serve para exibir as diferenças de um branch;
- Quando utilizado as diferenças do branch atual com o remoto serão exibidas no terminal;
- Podemos também verificar a diferença entre arquivos: **git diff <arquivo> <arquivo_b>**;

```$ git diff <nome_branch>``` -> exibi as diferenças do branch atual com outro branch ou um branch remoto;
```$ git diff main``` -> exemplo

```$ git diff <arquivo> <arquivo_b>``` -> exibi as diferenças de codigos entre arquivos;
```$ git diff HEAD:<nome_do_arquivo_a> <nome_do_arquivo_b>``` -> HEAD:<nome_do_arquivo_a> (arquivo presente no branch remoto), <nome_do_arquivo_b> (arquivo presente no branch atual) -> arquivos que estão com o codigo sendo comparados 
```$ git diff HEAD:a.txt a.txt``` -> exemplo

