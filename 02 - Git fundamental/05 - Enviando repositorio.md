# Enviando repositórios para o GH

- Podemos facilmente **enviar nossos repos** para o GitHub;
- Precisamos criar o projeto no GitHub, inicializar o mesmo no git em nossa máquina, sincronizar com o GH e enviar;
- E esta sequência que parece complexa é facilmente executada **por poucos comandos**;
- Vale lembrar que só fazemos **uma vez por projeto** este fluxo;
- Porém alguns comandos utilizados vão ser utéis ao longo do curso;

### GitHub
- Repositories -> New 

- Create a new repository:
    - Owner: (dono do repositorio)
    - Repository name: (nome do repositorio)
    - Description: (descrição do repositorio)
    - Public (repositorio publico)
    - Private (repositorio privado)
    - Initialize this repository with:
        - Add a README file (arquivo com uma descrição explicando tudo que o projeto faz)
        - Add .gitignore (arquivo descrevendo os arquivos que o GH deve ignorar)
        - Choose a license (quando quer atribuir ao software uma licença, por exemplo, a licença MIT)

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

