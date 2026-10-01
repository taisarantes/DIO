# Como gerar uma chave SSH?

- Abrir o terminal CMD ou Git Bash na pasta raiz do git (onde esta o arquivo .git do projeto), digitar o comando *ssh-keygen*
- O comando irá criar um repositório (por padrão) no caminho C/users/tais.arantes/.ssh
- Ele permite definir uma senha para acessar os arquivos, porém não é uma etapa obrigatória
- Após a etapa opcional de senha, ele criará dois arquivos no diretório .ssh, ambos com o nome sendo o id da chave ssh, sendo a chave privada um arquivo e a chave pública um arquivo .pub

## Adicionando a chave SSH ao GitHub

- Abrir o terminal CMD ou Git Bash na pasta .ssh
- Digitar o comando *cat [arquivo da chave pública]* para exIbir o conteudo do arquivo da chave pública, que será incluída no GitHub
- Após copiar o valor do arquivo, acessar as configurações do seu perfil no GitHub no caminho: **Settings > SSH and GPG keys**
- Clicar em **New SSH Key**
- Definir um **Título**, o **Tipo de Chave** (chave de autenticação) e colar a chave pública no campo **Chave** e clicar em **Add SSH Key**

## Clone com HTTPS x SSH

Caso o clone tenha sido feito utilizando HTTPS, não será possível realizar push utilizando a chave SSH. Se necessário, seguindo esses passos, é possível trocar um repositório HTTPS para SSH:
- Ir no repositório e copiar o link SSH
- Na pasta raiz do projeto, pelo terminal ou Git Bash, digitar o comando *git remote set-url [URL]*