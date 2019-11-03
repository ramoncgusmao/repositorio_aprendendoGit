
# git

## add

- **git add <arquivo>** = adiciona o arquivo a staging area 
- **git add .** = adiciona todos os arquivos modificados a staging area
- **git add --all** = adiciona todos os arquivos até os removidos.
- **git add -A** = adiciona todos os arquivos até os removidos.
- **git add -f** = força para adicionar arquivos.
- **git add -f <file>** = para forçar um arquivo.

## branch

- **git branch** = apresenta todas as branch 
- **git branch <nome>** = cria uma nova branch
- **git branch -m <nome>** = muda o nome da branch.
- **git branch -D <nome>** = remove a branch pode ser removidas varias de uma vez.
- **git branch --orphan <nome>** = cria uma branch vazia limpa.
- **git branch <commit>** = ele volta as alterações para esse commit.

 ## checkout
- **git checkout <nome>** = muda para a branch
- **git checkout -b <nome>** = cria uma branch e muda pra ela
- **git checkout <branch> -b <nome>** = cria uma branch a partir de outra branch e muda pra ela
- **git checkout <commit> -b <nome>** = cria uma branch a partir de um commit e muda pra ela
- **git checkout <commit>** = volta para o commit, sem criar branch
    
 ## clone
- **git clone <repositorio>** = busca um repositorio e baixa seus arquivos para sua maquina

 ## commit
- **git commit** = adiciona o arquivo ao repositorio mas abre um editor para adicionar uma mensagem
- **git commit -m <mensagem>** = permite adicionar uma mensagem ao commit
- **git commit -am  <mensagem>** = commit direto sem precisar adicionar na staging area
- **git commit -a -m  <mensagem>** = commit direto sem precisar adicionar na staging area
- **git commit --amend** = sobrescreve o ultimo commit

## config
- **git config --global core.excludesfile** = para indicar um .gitignore global
- **git config --global core.editor** = para selecionar um editor padrão
- **git config --global credential.helper cache** = salva a senha no computador.
- **git config --global credential.helper 'cache --timeout=<tempo>'** = salva a senha no computador por um tempo determinado
- **git config --global user.email <email>** = configura o email global para todos os projetos
- **git config --global user.name <nome>** = configura o nome de um usuario global para todos os projetos
- **git config user.email <email>** = configura o email de um projeto
- **git config user.name <nome>** = configura o nome de um usuario de um projeto
- **git config --list** = apresenta a lista com as configurações do git
- **git config --unset** = remove alguma credencial

## diff  
- **git diff**= apresenta as alterações realizadas,
- **git diff --staged**= diferenças entre a staged e o repository,
- **git diff <commit>**= apresenta as modificações feitas do commit para o atual
-**git diff <commit> <commit>**= mostra as modificacoes que foram feitas entre os commit
- **git diff -w**= remove os espaços
## fetch 
- **git fetch <repository>**= baixa as modificações de outro repositorio diferente do origin
        

## init

- **git init** = inicia o repositorio  
- **git init --bare** = cria Repositorios para o servidor


## log

- **git log** = apresenta dados do commit atual.  
- **git log --name-status** = apresenta todos os arquivos modificados no log dos commit  
- **git log --pretty=oneline** = o log vem só em uma linha.  
- **git log --abrev-commit** = reduz o nome do commit pra trazer só os primeiro catacteres.  
- **git log --stat** = apresenta um log mais detalhado.  
- **git log -p -<numero>** = traz a quantidade de commits especificados completo.  
- **git log --pretty=format** = mediante uma formatação ele devolve o commit customizado.    
  
## merge
- **merge <branch>** junta as branch atual que voce está com a que você solicitou
- **merge --abort** desfazer o merge
## push 
    
- **push <origin> <branch>** sobe os commit de uma branch para o repositorio,
- **push <origin> <branch> --delete** deleta a branch no repositorio
- **push <origin> :<branch>** deleta a branch no repositorio

## remote
- **remote -v** mostra o caminho do repository
- **remote add <local> <repository>** vincula os arquivos locais a um repositorio
- **remote set-url <origin> <repositorio>** modifica o repositorio vinculado atual pelo novo

## rm
- **git rm <arquivo>** = remove o arquivo do repository
- **git rm -r** = remove um diretorio
- **git rm -rf** = remove todos os arquivos da staging area
- **git rm -rf --cached** = remove todos os arquivos sem remover localmente
- **git rm -rf <diretorio>** = remove todos os arquivos do diretorio

## stach
- **git stach** = cria uma stach
- **git stach list** = lista as stach na fila
- **git stach apply** = busca a primeira stash da fila
- **git stach drop <nome>** = deleta uma stash
- **git stach git stach pop** = busca a primeira stash da fila e retira ela da area de stach
     

## status

- **git status** = mostra a situação atual

# rm
- **rm <arquivo>** = remove o arquivo da staging area
- **rm -r** = remove um diretorio
  


    

_obs: esses são os comandos que eu mais uso, fique a vontade para colocar comandos nos issues ou fazer um pull request adicionando mais comandos e me marcar na mensagem, assim eu aproveito e treino utilizar o git, obrigado pela atenção_