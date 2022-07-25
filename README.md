# comandos-git

### Atalhos
- Cria a branch e já navega para ela
> git checkout -b nomeBranch 

### Configuração inicial: definir nome e email de usuário
- git config --global user.name "NomeDeUsuário"
- git config --global user.email "email@gmail.com"

### Inicializar um repositório
- git init

### Adicionar os arquivos para o cotrole de versão
- git add .
- git add nomeDoArquivoOuPasta

### Visualizar o status dos arquivos
- git status

### Criar um ponto na história do projeto
- git commit -m "Mensagem do commit"

### Ver quais alterações foram feitas nos arquivos do projeto
- git diff

### Salvar temporariamente alterações no projeto
- Salvar as alterações feitas após o último commit, temporariamente
> git stash
- Visualizar todos os "stashs" disponíveis
> git stash list
- Visualizar detalhes de um stash especifico
> git stash show -p stash@{1}
- Aplicar novamente as alteraççoes salvas no stash ao projeto, sem apagar o stash cirado
> git stash apply
- Aplicar um stash especifico ao projeto
> git stash apply stash@{2}
- Aplicar o último stash ao projeto, apagando ele em segudida
> git stash pop
- Deletar um stash específico
> git stash pop

### Trabalhando com Logs
- Visualizar todos os commits realizados no projeto
> git log
- Visualização simplificada dos commits realizados no projeto
> git log --oneline
- Visualizar todas as alterações feitas em cada commit realizado no projeto
> git log -p
- Visualizar cada alteração, em cada commit de um arquivo especifico
> git log -p nomeDoArquivo
- Visualizar apenas os commits de merge
> git log --merges
- Visualizar apenas os 5 ultimos commits
> git log -5

### Voltar para um determinado ponto na história
- git checkout codigoDoCommit

### Comandos para manipular branchs
- Criar uma nova branch: 
> git branch nomeDaNovaBranch
- Deletar um branch:
> git branch -D nomeDoBranch
- Visualizar todos os branchs existentes:
> git branch
- Alterar o branch em que está:
> git checkout nomeDoBranch
- Passar os commits de um branch para outro:
> git merge nomeDoBranch

### Git + GitHub
- Vincular o repositório local á um remoto:
> git remote add origin URLdoRepositório
- Listar todos os pontos remotos:
> git remote -v
- "Empurra" os pontos na história do projeto local para o remoto:
> git push origin main
- Clonar um reposiorio remoto para o próprio computador:
> git clone URL nomeDaPastaOuBranco
- "Puxa" as alterações recentes do repositório remoto para o projeto local:
> git pull origin main


