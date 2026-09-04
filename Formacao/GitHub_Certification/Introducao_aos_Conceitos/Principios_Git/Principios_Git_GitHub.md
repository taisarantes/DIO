# Introdução GIT e GITHUB - Princípios e Conceitos

### Apesar de serem duas ferramentas integradas, é importante destacar a diferença entre elas

O GIT é um sistema de controle de versão distribuído (DVSC). Um controle de versão distribuído é a copia do código fonte localmente na nossa máquina, possibilitando que, em um projeto com vários desenvolvedores, cada um pode editar a versão do código que está copiada na máquina, para depois juntar as alterações de cada um com um comando merge, por exemplo. Com esse controle de versão, caso haja aglum erro ou bug em uma atualização do código, é possível voltar para uma versão mais estável.
O GITHUB é uma plataforma online, na nuvem, que serve como um repositório para guardar o código fonte, não dependendo de pen-drives ou de servidores, facilitando a troca de versões e a colaboração entre os desenvolvedores. 

### Para deixar seu git mais seguro, é sempre interessante realizar essas configurações iniciais

Para cofnigurar seu usuário:
- git config --global user.name "___"

Para configurar seu email:
- git config --global user.email "___"

Para validar se as configurações globais estão corretas:
- git config --list 

### Principais comandos

Inicia um novo repositório Git no diretório atual:
- git init

Clona um repositório Git existente para o diretório atual:
- git clone [URL]

Adiciona alterações ao índice (staging area) para prepará-las para o commit:
- git add .

Realiza um commit com as alterações adicionadas, incluindo uma mensagem obrigatória que descreve as alterações feitas:
- git commit -m "mensagem"

Exibe o estado atual do repositório, indicando quais arquivos foram modificados, adicionados ou removidos:
- git status

Mostra o histórico de commits do repositório:
- git log

Lista todas as branchs locais e destaca a branch atual:
- git branch

Cria uma nova branch:
- git branch [branch]

Altera para uma branch específica:
- git checkout [branch]

Combina as alterações de uma branch para a branch atual:
- git merge [branch]

Atualiza o repositório local com as alterações do repositório remoto:
- git pull

Envia os commits locais para o repositório remoto:
- git push [remote] [branch] 

Lista os repositórios remotos configurados:
- git remote -v

Recupera as últimas alterações do repositório remoto, mas não faz merge automaticamente:
- git fetch

Desfaz as alterações no arquivo especificado, removendo-o do índice:
- git reset [arquivo]

Remove um arquivo do repositório e o inclui no próximo commit:
- git rm [arquivo]

Mostra as diferenças entre as alterações que ainda não foram adicionadas ao índice:
- git diff

Adiciona um repositório remoto com um nome específico:
- git remote add [nome-remoto] [URL]

Executado para efetuar push das alterações locais para o repositório online:
- git push add origin main






