# Comandos Básicos do Git

-git clone, como no nome cria uma duplicata de repositórios na pasta local
-git commit, grava alterações de uma nova versão feita 
-git pull, "puxa" as alterações do repositório local para o remoto (busca e mescla)
-git push, "empurra" as alterações do repositório local para o remoto
-git status: ver os status
-git log: ver todos os commits
-git commit --amend -m: serve para mudar o comentário do último commit
-git reset --soft: pega os arquivos do commit e coloca eles na área de preparação
-git reset --mixed: pega os arquivos do commit e coloca eles na área de trabalho, sendo listados como untracked files
-git reset --hard: pega os arquivos do commit e simplesmente os exclui
-git reflog: mostra o histórico do git log
-git reset <nome do arquivo> ou git restore --staged <nome do arquivo>: servem para remover arquivos do commit e colocá-los na área de preparação

## Para enviar algo para um repositório remoto são necessárias algumas etapas 
 *basta primeiro criar o repositório na sua máquina local
 *adicionar algum arquivo (mais comum README.md)
 *iniciar o git init no repositório
 *usar o comando git add .
 *criar um commit
 *criar o repositório no github
 *git remote add origin <link do repositório remoto>


-git checkout -b <nome da branch>, para colocar uma nova branch acoplada a branch atual
-git chechout <nome da branch>, muda para a branch escolhida
-git branch -v: lista o último commit de cada branch
-echo "#<nome do arquivo>" > <nome do arquivo e o seu tipo"> serve para criar arquivo, tipo touch README.md
-git merge <nome da branch a ser "ajuntada">
-git branch -d <nome da branch> para excluir uma branch
-giut fetch: baixa as alterações
-git diff <branch padrão>/<branch a ser comparada>: mostra comparações entre as branches
-git merge <branch padrão>/<branch a ser mesclada>: serve para mesclar alterações do repo remoto ao repo local
-git clone <url> --branch <nome da branch> --single-branch: serve para clonar uma branch específica do repositório, se não especificado somente a branch main será clonada