
Listagem pra ver se tem alguma chave ssh no seu  pc 


1. Abra Git Bash.
2. Insira `ls -al ~/.ssh` para ver se as chaves SSH existentes estão presentes.
    
   ```shell
    $ ls -al ~/.ssh
    # Lists the files in your .ssh directory, if they exist
    ```
    
    Verifique a listagem do diretório para verificar se você já tem uma chave SSH pública. Por padrão, os nomes de arquivos de chaves públicas com suporte para o GitHub são um dos seguintes.

- _id_rsa.pub_
- _id_ecdsa.pub_
- _id_ed25519.pub_

**Dica**: se você receber um erro indicando que _~/.ssh_ não existe, você não terá um par de chaves SSH existente no local padrão. Você pode criar um novo par de chaves SSH na próxima etapa.


