# Transformando o repo para arquivo

- Com o comando **git archive** podemos transformar o repo para um arquivo compactado, por exemplo;
- O comando é **git archive --format zip --output master_files.zip master**
- E então a master vai estar zipada no arquivo master_files.zip´

```$ git archive --format <formato_da_pasta> --output <nome_da_pasta>.<formato_da_pasta> <branch>``` -> transforma o repo em um arquivo compactado
```$ git archive --format zip --output master_files.zip master``` -> exemplo