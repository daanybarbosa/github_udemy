# Ignorando arquivos e diretórios no projeto

- Uma técnica muito utilizada é **ignorar arquivos do projeto**;
- Devemos inserir um arquivo chamado **.gitignore** na raiz do projeto;
- Nele podemos inserir todos os arquivos que não devem entrar no versionamento;
- Isso é útil para **arquivos gerados automaticamente** ou arquivos que contêm **informações sensíveis**;


**Exemplo**
__No arquivo: .gitignore__
d.txt -> ira ignorar o arquivo d.txt dos commits do projeto
node_modules/* -> todos os arquivos dentro do node_modules serão ignorados 


```$ git status```
```$ git add .``` -> adicionar o arquivo .gitignore
```$ git commit -a -m "Adicionando git ignore"```
```$ git push```
