# Reflog

- O **git reflog** vai mapear todos os seus passos no repositorio, até uma mudança de branch é inserida neste log;
- Já o **git log**, que vimos anteriormente, apenas armazena os commits de um branch;
- Os **reflogs ficam salvos até expirar**, o tempo de expiração padrão é de 30 dias (dá para aumentar esse prazo);

```$ git reflog``` -> vai exibir todos os passos no repositorio, como a mudança de um branch, é um comando mais completo do que o git log, ele possui um prazo padrão de expiração que é de 30 dias.
